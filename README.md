
# OLTP-AdventureWorks2019-MySQL
This is the MySQL dump of AdventureWorks sample databases.<br>

How this was created:<br>
Imported into SQL Server 2019 using Azure Data Studio and then migrated using MySQL Workbench.

How can you import it into MySQL:<br>
If you're already logged in into mysql client then:
```
mysql> create database your_database_name;
mysql> use your_database_name;
mysql> source /home/sysadmin/Downloads/AdventureWorks2019.sql;
```
Otherwise you can directly import it using terminal:
**Note:** `your_database_name` db already needs to be present/created in MySQL.
```
mysql -u username -p your_database_name < /home/sysadmin/Downloads/AdventureWorks2019.sql
```
