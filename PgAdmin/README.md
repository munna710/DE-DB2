# ERD diagram shows the schema of the complete eBooks database
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/eBooks/eBooks_schema_complete.png)
## Restore a database schema and data
### create a database
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/1.6.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/1.6.2.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/1.7.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/1.8.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/1.8.5.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/1.8.7.png)
## Create and execute a view
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/2.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/2.2.png)
### SELECT books.title, books.rating, publishers.name 
### FROM books INNER JOIN publishers ON books.publisher_id = publishers.publisher_id
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/2.3.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/2.4.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/2.5.png)
## Create and execute a materialized view
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/3.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/3.2.png)
### SELECT books.title, books.rating, publishers.name 
### FROM books INNER JOIN publishers ON books.publisher_id = publishers.publisher_id
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/3.3.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/3.4.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/3.5.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Views%20in%20PostgreSQL/images/3.6.png)
