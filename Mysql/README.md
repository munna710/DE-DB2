# entity relationship diagram (ERD) shows the schema of the Sakila database:
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/sakila/sakila_ERD.jpg)
## to fetch the sakila_mysql_dump.sql file
- wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/sakila/sakila_mysql_dump.sql
## create a database
- create database sakila;
- use sakila;
## Restore the sakila mysql dump file (containing the sakila database table definitions and data) to the newly created empty sakila database. A dump file is a text file that contains the data from a database in the form of SQL statements. This file can be imported using the command line with the following command:
- source sakila_mysql_dump.sql;
- Note: You can use the source command to restore the database dump file within the mysql command prompt. To restore the database dump file outside of the mysql command prompt, you can use the mysql --host=127.0.0.1 --port=3306 --user=root --password sakila < sakila_mysql_dump.sql command after quitting the mysql command prompt session with command \q.
## Explore and query tables
- SHOW FULL TABLES WHERE table_type = 'BASE TABLE';
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20MySQL%20command%20line/images/C.1.png)
-The Table_type for these tables is BASE TABLE. BASE TABLE means that it is a table as opposed to a view (VIEW) or an INFORMATION_SCHEMA view (SYSTEM VIEW).
## Explore the structure of the staff table
- DESCRIBE staff;
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20MySQL%20command%20line/images/C.2.png)
- SELECT * FROM staff;
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20MySQL%20command%20line/images/C.3.png)
## dump/backup the staff table from the database
- mysqldump --host=127.0.0.1 --port=3306 --user=root --password sakila staff > sakila_staff_mysql_dump.sql
## To view the contents of the dump file
- cat sakila_staff_mysql_dump.sql

