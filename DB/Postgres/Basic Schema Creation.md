Below is an example of initializing a DB with a user and a schema. Schemas are a nice way of logically grouping your tables (you can still cross query between schemas). It is important to note you **do not** have to create a user, this is just if you want to lock down access.

Also notice the *GRANT* at the bottom of the statement. If this is not done after the creation of all the tables, the user will not be granted to access. Think of it as giving access to whatever existing tables are there.

- [Source](https://www.postgresql.org/docs/current/ddl-schemas.html)

```sql
CREATE USER ds_auth WITH PASSWORD 'password';
CREATE SCHEMA ds_auth AUTHORIZATION ds_auth;

CREATE TABLE ds_auth.users
(
    id         SERIAL PRIMARY KEY,
    username   VARCHAR(100) NOT NULL UNIQUE,
    password   VARCHAR(255) NOT NULL,
    email      VARCHAR(255) NOT NULL UNIQUE,
    created_at TIMESTAMP    NOT NULL DEFAULT NOW(),
    updated_at TIMESTAMP    NOT NULL DEFAULT NOW()
);

create TABLE ds_auth.sessions
(
    id         SERIAL PRIMARY KEY,
    user_id    INTEGER      NOT NULL UNIQUE REFERENCES ds_auth.users (id),
    session_id VARCHAR(25)  NOT NULL UNIQUE,
    token      VARCHAR(255) NOT NULL UNIQUE,
    created_at TIMESTAMP    NOT NULL DEFAULT NOW(),
    updated_at TIMESTAMP    NOT NULL DEFAULT NOW()
);

GRANT ALL PRIVILEGES ON ALL TABLES IN SCHEMA ds_auth TO ds_auth;

INSERT into ds_auth.users
    (username, password, email)
values ('admin', 'admin', 'admin@localhost');
```