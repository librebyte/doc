---
Title: "PostgreSQL basic commands"
Date: 2017-06-01 20:06:32
Categories: [data base]
tags: [postgresql]
Authors: sedlav
---

## Connect to the database with default user

```sh
$ sudo -u postgres psql
```

## Create user

```sql
CREATE USER username WITH PASSWORD 'MYPASS';
```

## Set super privileges to specific user

```sql
ALTER USER username WITH SUPERUSER;
```

## Create a database

```sql
CREATE DATABASE dbname OWNER username;
```

## Drop database

```
DROP DATABASE dbname;
```

## List databases

```
\l
```

## Import a data base

```
$ psql username  -h hostname -d dbname < dump.sql
```

## Change DATABASE

```
\c dbname;
```

## Create Postgis extension

```sql
CREATE EXTENSION Postgis;
```

## List tables

```
\dt
```

## Quit from Postgre console

```
\q
```