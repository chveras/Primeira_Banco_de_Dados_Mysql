# Primeira_Banco_de_Dados_Mysql
Primeira tabela de dados criada no prompt mysql


C:\Arquivos de Programas\mysql\MySQL Server 8.0\bin>mysql -u root -p
Enter password: *********
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 15
Server version: 8.0.30 MySQL Community Server - GPL

Copyright (c) 2000, 2022, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> cls
    ->
    -> clr
    -> cls
    -> show databases;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'cls

clr
cls
show databases' at line 1
mysql> create database Dbteste;
Query OK, 1 row affected (0.07 sec)

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| dbteste            |
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.06 sec)

mysql> drop dbteste;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'dbteste' at line 1
mysql> ls
    -> help;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'ls
help' at line 1
mysql> \c
mysql> '\c'
    -> use dbteste
    ->
    -> mysql
    -> show databases
    ->
    -> use dbteste;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near ''\c'
use dbteste

mysql
show databases

use dbteste' at line 1
mysql> \c;
ERROR:
No query specified

mysql> drop database dbteste
    -> drop database dbteste;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'drop database dbteste' at line 2
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| dbteste            |
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.00 sec)

mysql> use database;
ERROR 1049 (42000): Unknown database 'database'
mysql> use database dbteste
ERROR 1049 (42000): Unknown database 'database'
mysql> use database dbteste;
ERROR 1049 (42000): Unknown database 'database'
mysql> use dbteste;
Database changed
mysql> show tables;
Empty set (0.02 sec)

mysql> drop database dbteste;
Query OK, 0 rows affected (0.03 sec)

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
4 rows in set (0.00 sec)

mysql> c;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'c' at line 1
mysql> \c;
ERROR:
No query specified

mysql> \h;

For information about MySQL products and services, visit:
   http://www.mysql.com/
For developer information, including the MySQL Reference Manual, visit:
   http://dev.mysql.com/
To buy MySQL Enterprise support, training, or other products, visit:
   https://shop.mysql.com/

List of all MySQL commands:
Note that all text commands must be first on line and end with ';'
?         (\?) Synonym for `help'.
clear     (\c) Clear the current input statement.
connect   (\r) Reconnect to the server. Optional arguments are db and host.
delimiter (\d) Set statement delimiter.
ego       (\G) Send command to mysql server, display result vertically.
exit      (\q) Exit mysql. Same as quit.
go        (\g) Send command to mysql server.
help      (\h) Display this help.
notee     (\t) Don't write into outfile.
print     (\p) Print current command.
prompt    (\R) Change your mysql prompt.
quit      (\q) Quit mysql.
rehash    (\#) Rebuild completion hash.
source    (\.) Execute an SQL script file. Takes a file name as an argument.
status    (\s) Get status information from the server.
system    (\!) Execute a system shell command.
tee       (\T) Set outfile [to_outfile]. Append everything into given outfile.
use       (\u) Use another database. Takes database name as argument.
charset   (\C) Switch to another charset. Might be needed for processing binlog with multi-byte charsets.
warnings  (\W) Show warnings after every statement.
nowarning (\w) Don't show warnings after every statement.
resetconnection(\x) Clean session context.
query_attributes Sets string parameters (name1 value1 name2 value2 ...) for the next query to pick up.
ssl_session_data_print Serializes the current SSL session data to stdout or file

For server side help, type 'help contents'

mysql> \c
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
4 rows in set (0.00 sec)

mysql> create database firstExample;
Query OK, 1 row affected (0.00 sec)

mysql> use firstexampla
ERROR 1049 (42000): Unknown database 'firstexampla'
mysql> use firstExample;
Database changed
mysql> c;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'c' at line 1
mysql> \c
mysql> \c;
ERROR:
No query specified

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| firstexample       |
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.00 sec)

mysql> use firstExample;
Database changed
mysql> create table periodicos(
    -> id int auto_increment primary key,
    -> nome_periodico varchar(20),
    -> issn INT,
    -> id_editora INT
    -> );
Query OK, 0 rows affected (0.04 sec)

mysql> show table;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '' at line 1
mysql> show tables;
+------------------------+
| Tables_in_firstexample |
+------------------------+
| periodicos             |
+------------------------+
1 row in set (0.00 sec)

mysql> CREATE TABLE editora(
    -> id integer auto_increment,
    -> nome_editora varchar(120) unique,
    -> pais varchar(5),
    -> primary key(id),
    -> );
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near ')' at line 6
mysql> CREATE TABLE editora(
    ->     -> id integer auto_increment,
    ->     -> nome_editora varchar(120) unique,
    ->     -> pais varchar(5),
    ->     -> primary key(id),
    -> \c
mysql> CREATE TABLE editora(
    ->     -> id integer auto_increment,
    ->     -> nome_editora varchar(120) unique,
    ->     -> pais varchar(5),
    ->     -> primary key(id),
    ->     -> );\c
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '-> id integer auto_increment,
    -> nome_editora varchar(120) unique,
    -> pa' at line 2
mysql> CREATE TABLE editora(
    ->     -> id integer auto_increment,
    ->     -> nome_editora varchar(120) unique,
    ->     -> pais varchar(5),
    ->     -> primary key(id),
    ->     -> primary key(id),\c
mysql> CREATE TABLE editora(
    ->     -> id integer auto_increment,
    ->     -> nome_editora varchar(120) unique,
    ->     -> pais varchar(5),
    ->     -> primary key(id),
    -> \c
mysql> create table editora(
    -> id interger auto_increment,
    -> nome_editora varchar(120) unique,
    -> pais varchar(5),
    -> primary key(id)
    -> );
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'interger auto_increment,
nome_editora varchar(120) unique,
pais varchar(5),
prim' at line 2
mysql> create table editora(
    -> id integer auto_increment,
    -> nome_editora varchar(120) unique,
    -> pais varchar(5),
    -> primary key(id)
    -> );
Query OK, 0 rows affected (0.03 sec)

mysql> show tables;
+------------------------+
| Tables_in_firstexample |
+------------------------+
| editora                |
| periodicos             |
+------------------------+
2 rows in set (0.00 sec)

mysql> alter table periodicos add constraint fk_editora_periodico foreign key (id_editora) references editora(id);
Query OK, 0 rows affected (0.06 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> insert into editora (nome_editora, pais) values ('IEE', 'EUA'), ('DatascienceMagazine', 'EUA');
Query OK, 2 rows affected (0.01 sec)
Records: 2  Duplicates: 0  Warnings: 0

mysql> select * from editora;
+----+---------------------+------+
| id | nome_editora        | pais |
+----+---------------------+------+
|  1 | IEE                 | EUA  |
|  2 | DatascienceMagazine | EUA  |
+----+---------------------+------+
2 rows in set (0.00 sec)

mysql> select * from periodicos;
Empty set (0.00 sec)

mysql> insert into periodicos(nome_periodico, issn, id_editora) values ('Special Issue', '12345678', '1');
Query OK, 1 row affected (0.00 sec)

mysql> select * from periodicos;
+----+----------------+----------+------------+
| id | nome_periodico | issn     | id_editora |
+----+----------------+----------+------------+
|  1 | Special Issue  | 12345678 |          1 |
+----+----------------+----------+------------+
1 row in set (0.00 sec)

mysql> insert into periodicos(nome_periodico, issn, id_editora) values ('Special Issue', '12345678', '1');
Query OK, 1 row affected (0.00 sec)

mysql> select * from periodicos;
+----+----------------+----------+------------+
| id | nome_periodico | issn     | id_editora |
+----+----------------+----------+------------+
|  1 | Special Issue  | 12345678 |          1 |
|  2 | Special Issue  | 12345678 |          1 |
+----+----------------+----------+------------+
2 rows in set (0.00 sec)

mysql> drop id(2);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'id(2)' at line 1
mysql>