**If you are running postgres within a container make sure to first connect to it either as the DB user or switch to the db user once connected.**

If you have connected to the container already run the following as per note above.

```sh
su {user}
```

## Run psql

Now that you are connected to the container or are already the correct user you can then connect to the db as the specified user. To do so run the below:

```sh
psql -U {user} {db}
```

You can now execute sql scripts as per normal

```sql
select * from {table}
```

Here are some useful commands to validate your db once connected:

```psql
\dt
\d {table}
```
