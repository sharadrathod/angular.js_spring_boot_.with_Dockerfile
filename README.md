# launch rds mysql db instance 

- login in cloudshell:
```sh
  mysql -h <endpoint_of_db_instance> -u <user_name> -p<password>
``` 
- create database in mysql 
```sh
CREATE DATABASE springbackend;
```
- exit from mysql
```sh
exit
```
- clone github repo 
```sh
git clone https://github.com/sharadrathod/angular_springboot_project.git 
``` 
- create shchema in mysql 
```sh
mysql -h <endpoint> -u <user> -p<password> springbackend < springbackend.sql 
```
Login to the database again:
```sh
mysql -h <endpoint> -u <user> -p<password> 
```
- View all the databases created:
  ```sh
  SHOW DATABASES;
  ```
  - Use the database:
  ```sh
  use springbackend;
  ```
  - View the tables created:
  ```sh
  SHOW tables;
  ```
  - View the content of the table:
  ```sh
  select * from tbl_workers;
  ```