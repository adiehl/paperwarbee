# paperwarbee
Easy invoice and business correspondence suite

# setup instructions
## create database and database user (mysql)
start your favorite mysql-client
```
mysql -uroot -p
```
in mysql, enter these commands (change user and password in a productive environment, please)
```
CREATE DATABASE paperwarbee;
GRANT ALL PRIVILEGES ON paperwarbee.* TO 'paperwarbee'@'localhost' IDENTIFIED BY 'paperwarbee';
```
import the schema
```
mysql -upaperwarbee -ppaperwarbee paperwarbee < db/Schema.sql
```
