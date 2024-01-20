# Entity Relation Diagram (ERD) diagram
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/sakila/sakila_ERD.jpg)
##  fetch the sakila_pgsql_dump.sql file
wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/sakila/sakila_pgsql_dump.sql
## Create a database
- create database sakila;
- \connect sakila;
- \include sakila_pgsql_dump.sql;
## Explore and query tables
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20PostgreSQL%20command%20line/images/1.10.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20PostgreSQL%20command%20line/images/1.11.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Getting%20started%20with%20PostgreSQL%20command%20line/images/1.12.png)
## to dump/backup the store table from the database
- pg_dump --username=postgres --host=localhost --password --dbname=sakila --table=store --format=plain > sakila_store_pgsql_dump.sql
## To view the dump file within the terminal
- cat sakila_store_pgsql_dump.sql

