#Installs

```brew
brew install mysql
```

look here for new drivers for sql
https://github.com/golang/go/wiki/SQLDrivers

##You always need to start mysql before use

```brew
brew services start mysql
```

Mysql is not secure to secure it run :: can skip this step

```sql
mysql_secure_installation
```

To run the mysql db server run

```sql
create database <whatever you want to name it>
```

At the CLI log into my database management system 'DBMS'

```sql
mysql -u root
```

Create a new database

```sql
create database recordings;
```

If you need to navigate to the DB run

```sql
use recordings;
```

##Create MySql scheme

You have finally created a database now you can create a new file.sql to build out the scheme <create-table.sql>

Run the scheme file

```sql
source create-tables.sql
```

If you want to see what databases have been created

```sql
show databases;
```

How to show users
sel

```sql
SELECT User, Host, Password FROM mysql.user;
SELECT * FROM mysql.user;
```

shows current user

```sql
select user();
```
# go_mysql_firstGo
