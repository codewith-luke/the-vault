---
title: Create and Seed Your Postgres Database in Minutes with Docker
published: false
description: In this tutorial, we'll show you how to quickly create a Postgres database using Docker and Go. We'll also demonstrate how to seed your database with fake data using Go, which can be useful for testing and development purposes. By the end of this tutorial, you'll have a fully functional Postgres container that you can use for your next project.
tags: Go, Postgres, Docker, Database
# cover_image: https://direct_url_to_image.jpg
# Use a ratio of 100:42 for best results.
# published_at: 2022-12-09 11:03 +0000
---

## Table of Contents

-  What is Database Seeding and Why?
-  Building Your Postgres Docker Container
    -   Prerequisites
    -   Creating the Docker Container
    -   Connecting to our DB
-   Structuring Your DB with Go Migrate
    -   Generating Our Migration Scripts
    -   Running our Scripts
-   Populating Your DB with Go Faker
    -   Generating Fake Data
    -   Inserting Fake Data into the Database
- Summary

This will help us understand the importance of creating silo'ed development environments that allow us to quickly iterate, create scenarios and test. In this article we will focus on using Go as our language to programatically seed our data. However there are tools in other languages to achieve the same results. Whatever your preference, this article just hopes to achieve bringing light to how you can go about it.

# What is Database Seeding and why

Database seeding is the process of adding initial data to a database. This is often done for testing or development purposes, as it allows developers to work with a sample dataset without having to worry about corrupting real data. Database seeding can be useful for testing the functionality of a database, as well as for experimenting with different queries and data structures. In general, seeding a database with fake data can help ensure that the database is working properly and can be useful for a variety of purposes.

One important aspect we want to ensure is that it is quick and easy to reboot and create these scenarios or get us back to a stable point.

# 1) Building Your Postgres Docker Container

Before we can start seeding our database we first have to get our container up and running.

### Prerequisites

Before we begin with creating a container we need to ensure that we have [Docker installed and running](https://docs.docker.com/get-started/).

Now you will not need to worry about getting too advanced with Docker features. So if you are not very well versed in Docker do not worry. 

In short we are going to use a predefined Docker image for Postgres and then modify and put some data into it.

### Creating the Docker Container

So to start we want to create our bare bone Postgres container:

```sh
docker run --name my-db -e POSTGRES_PASSWORD=pwd -e POSTGRES_DB=database -d -p 5432:5432 postgres
```

This will create a new Docker container named "my-db" using the latest version of the Postgres image from Docker Hub. 

The `-e` flag is used to set the password for the default user (default is `postgres`) to mysecretpassword as well as creating us a database inside our container called 'database' (default is `postgres`). 

The `-d` flag specifies that the container should run in detached mode, running in the background. 

Then the `-p` flag is used to expose the port of our container and map it to our db, in this case it is a mapping of `5432 -> 5432`

To confirm it is running we can then run:

```sh
docker ps
```

### Connecting to our DB

So now that our container is up and running you may be asking yourself how do I connect to it or how do I know it is working?

We will now connect to our new Postgres container to then confirm that it is as we expect:

```sh
docker container exec -it my-db bash
```
Once connected to the container we can confirm all is running fine with:

```sh
psql -u {user} {db}
```

**NOTE: to exit this psql `\q` and hit enter**

So if you have followed the above you can swap out user for `postgres` and db for `database` or whatever you have named your instance.

Now you are able to execute and insert data into your new database.

If you prefer to just connect to the container and run queries direct you can modify the above:

```sh
psql -U {user} {db} -c "{SQL_QUERY}"
```

# 2) Structuring Your DB with Go Migrate

Now that we have got our database running we want to now populate it with some tables. 

This involves specifying the schema, which defines the structure and organization of the data, as well as any constraints or rules for the data. To do this we are going to use [Go Migrate](https://github.com/golang-migrate/migrate). 

Tools like Go migrate are typically used in database development to manage changes to the database schema over time. In our case we can make use of this tool to define our initial DB schema which will we then populate with the data we want.

## Generating Our Migration Scripts

Using the Go Migrate CLI we will first create our migration files in a folder of choice in our project.

```sh
migrate create -ext sql -dir db/schema -seq schema_init
```

This will create an up and down file. I recommend reading into how migration tools work. In short however. *Up* has to do with doing some form of change to your DB. Whereas *Down* has to do with reverting the changes. 

When using the CLI this will add some numbers to the front. This is used for internal tracking of what SQL scripts have been executed and what has not. So make sure to keep these.

Once you have generated your migration files we can then add our SQL scripts to structure our DB:

```sql
-- schema_init.up.sql

BEGIN;

-- Create the users table
CREATE TABLE users
(
    id       SERIAL PRIMARY KEY,
    username VARCHAR(255) NOT NULL,
    handle   VARCHAR(255) NOT NULL
);

COMMIT;

```

This will create 2 tables called *rooms* and *users*. You can create your structure however you want but this is just to show as an example.

## Running our Scripts

You can use the CLI to run a migration script while connecting to the DB directly. However in this example I am going to show you the code version.

TLDR; this is the end code:

```go
package main  
  
import (  
   "database/sql"  
   "fmt"   "github.com/golang-migrate/migrate/v4"   "github.com/golang-migrate/migrate/v4/database/postgres"   _ "github.com/golang-migrate/migrate/v4/source/file"  
   "github.com/joho/godotenv"   _ "github.com/lib/pq"  
   "log"   "os")  
  
func main() {  
   db, err := sql.Open("postgres", "postgres://postgres:mysecretpassword@localhost:5432/database?sslmode=disable")  
  
   if err != nil {  
      panic(err)  
   }  
  
   driver, err := postgres.WithInstance(db, &postgres.Config{})  
  
   if err != nil {  
      panic(err)  
   }  
  
   // NOTE: relative path to folder  
   m, err := migrate.NewWithDatabaseInstance(  
      "file://./db/dev",  
      "postgres", driver)  
  
   if err != nil {  
      panic(err)  
   }  
  
   err = m.Up()  
  
   if err != nil {  
      fmt.Println(err)  
   }  
}
```

Over here I have my main package that I can run. Using the `database/sql` and `golang-migrate` packages.

First we open a connection to our container DB, which includes the username, password, host, and port of the database, as well as the database name and SSL mode. We then create a new instance of the Postgres driver and uses it to connect to the database instance.

```go
   db, err := sql.Open("postgres", "postgres://postgres:mysecretpassword@localhost:5432/database?sslmode=disable") 
   
   driver, err := postgres.WithInstance(db, &postgres.Config{})  
```

Then we create a new instance of the migrate package, using the path to the migration files and the Postgres driver instance (In my case this is relative path to where I am executing this script). This allows the migrate package to access and manage the database schema using the provided migration files.

Finally, the code calls the `Up()` method on the migrate instance, which will apply any pending migration scripts to the database, updating the schema as necessary.

```go
   // NOTE: relative path to folder  
   m, err := migrate.NewWithDatabaseInstance(  
      "file://./db/dev",  
      "postgres", driver)  
  
   if err != nil {  
      panic(err)  
   }  
  
   err = m.Up()  
```

After this your running Postgres Container will now have its relevant schema set up. If you are wanting to change this at all. Create a *Down* script that removes these tables or simply delete you docker container and recreate it.

```sh
docker rm -f {container}
```

# Populating Your DB with Go Faker

Now that we have our DB and our Schema for our DB set and in place we now want to populate it with some fake data using [Go Faker](https://github.com/bxcodec/faker).

## Generating Fake Data

Go Faker is a handy little library that allows us to define a Struct, add some tags and it will then randomly generate data based on the tags we define.

In the example above we defined a `users` table. Now for simplicity we are going to generate ourselves a user and then insert that user into our DB.

First let's go ahead and define a user Struct:

```go
type User struct {
	Username string
	Handle   string
}
```

As you can see here there is nothing crazy going on. Just a simple struct with 2 properties. We can then dive into how faker can work in 2 different ways. Depending on what your needs are you may want to generate the data yourself or use aspects of faker to do it for us.

Let's modify our User model slightly by adding a faker tag to generate a username:

```go
type User struct {
	Username string `faker:"username"`
	Handle   string
}
```

The above has now defined that when we use Faker to generate our data that we want to use it's inbuilt generation to create a random username for us. There are a few other ways that you can ensure that it is unique. But there are many [tags you can use](https://github.com/bxcodec/faker/blob/master/example_with_tags_test.go).

To then generate using Faker we then can add the following piece of code:

```go
func createUser() User {
	user := User{}
	
	err := faker.FakeData(&user)
	
	if err != nil {
		fmt.Println(err)
	}
	
	return user
}
```

This method over here will now generate our user with a random username and a random string for their handle (if you do not define a tag it will generate randomly based on the type).

The alternative to the above is:

```go
func createUser() User {  
   user := internal.User{}  
   username := faker.Username()
   return user  
}
```

With the above approach there is no need for the tag.

## Inserting Fake Data into the Database

We now have a way of generating a user and inserting them into our DB. However how do we tie all this in together?

TLDR;

```go
package main  
  
import (  
   "database/sql"  
   "fmt"   "github.com/golang-migrate/migrate/v4"   "github.com/golang-migrate/migrate/v4/database/postgres"   _ "github.com/golang-migrate/migrate/v4/source/file"  
   "github.com/joho/godotenv"   _ "github.com/lib/pq"  
   "log"   "os")  
  
func main() {  
   db, err := sql.Open("postgres", "postgres://postgres:mysecretpassword@localhost:5432/database?sslmode=disable")  
  
   if err != nil {  
      panic(err)  
   }  
  
   driver, err := postgres.WithInstance(db, &postgres.Config{})  
  
   if err != nil {  
      panic(err)  
   }  
  
   // NOTE: relative path to folder  
   m, err := migrate.NewWithDatabaseInstance(  
      "file://./db/dev",  
      "postgres", driver)  
  
   if err != nil {  
      panic(err)  
   }  
  
   err = m.Up()  
  
   if err != nil {  
      fmt.Println(err)  
   }  

	user := createUser()
	insertUser(db, user)
}

func createUser() User {
	user := User{}
	
	err := faker.FakeData(&user)
	
	if err != nil {
		fmt.Println(err)
	}
	
	return user
}

func insertUser(db *sql.DB, user internal.User) int {  
   sqlStatement := "INSERT INTO users (username, handle) VALUES ($1, $2) RETURNING id;"  
  
   lastInsertId := 0  
   err := db.QueryRow(sqlStatement, user.Username, user.Handle).Scan(&lastInsertId)  
  
   if err != nil {  
      panic(err)  
   }  
  
   return lastInsertId  
}
```

Lets break down the new sections we just added to the above code:

```go
user := createUser()
insertUser(db, user)
```

In the main we then called our `createUser` method and then handed this over to another method who will then insert that user into our DB.

```go
func insertUser(db *sql.DB, user internal.User) int {  
   sqlStatement := "INSERT INTO users (username, handle) VALUES ($1, $2) RETURNING id;"  
  
   lastInsertId := 0  
   err := db.QueryRow(sqlStatement, user.Username, user.Handle).Scan(&lastInsertId)  
  
   if err != nil {  
      panic(err)  
   }  
  
   return lastInsertId  
}
```

The above is just taking our original connection when we did our schema setup and then executing a SQL query to insert into our users table.

This proceeds to then return the index that was last inserted in case we wanted to perform another action after.

# Summary

Hopefully all the above makes sense. To summarize everything:

- We created a bare bones Postgres Docker container
- Created scripts to structure our DB for us (Users table) using Go Migrate
- We then generated a random user with fake data using Go Faker
- Inserted this new user and returned the insertion ID

The example is not overly complicated however you can expand and add to it as you wish. Now as I said this is not something just for Go. Other languages have their own versions of these tools. The main takeaway is understanding their use cases and how they can be used together to create a development environment that is easy to modify and simple to reset should you need to! As always these things can be as complicated as you require.

If you liked this article be sure to follow or check out some of my socials. I [also stream on Twitch](https://www.twitch.tv/codingwithluke)  every Tuesday + Thursday at GMT+1.

  