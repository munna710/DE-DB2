# LAB-1
## structure of the myauthors table from the Books database
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/Books/Books_schema.png)
## create a database named Books
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.5.png)
## Create tables
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.6.png)
## Enter the table definition for the myauthors table
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.7.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.8.png)
## Load data into tables manually using the phpMyAdmin GUI
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.9.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.10.png)
##  Load data into tables using a text/script file.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.13.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.13.2.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20MySQL%20using%20phpMyAdmin/images/2.14.png)
# LAB-2
## entity relationship diagram (ERD) shows the current status of the schema of the eBooks database
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/eBooks/eBooks_schema_mysql_incomplete.png)
## load the eBooks_mysql_dump.sql
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/6.png)

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/7.png)
### Primary Keys: A primary key is a column or group of columns that uniquely identify every row in a table. They constrain the table by only accepting unique, non-NULL values for that column. Non-NULL data is data where the values exist.

Creating a primary key on a table automatically creates an index on the key. You will create a primary key for the author table to uniquely identify every row in the table. You will set the author_id column of the author table as a primary key.

- In the tree-view, click the authors table. Switch to the Structure tab and make sure you are inside Table structure subtab.
- Check the author_id column.
- Click the Primary option.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/8.png)
### Auto-increment: Auto-increment enables a unique number to be generated automatically when a new record is inserted into a table. Often this is used for the primary key field to be created automatically every time a new record is inserted. You will set the auto-increment feature for the primary key of the author table.

In the tree-view, click the authors table. Switch to the Structure tab and make sure you are inside the Table structure subtab.
Check the author_id column.
- Click the Change option.
- Check A_I option (A_I = Auto_Increment).
- Click Save.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/9.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/9.2.png)
### Null constraints: By default, a column can hold NULL values. If you do not want a column to have a NULL value, you can restrict the column from having a NULL value. You will restrict the first_name column of the authors table from having a NULL value.

In the tree-view, click the authors table. Switch to the Structure tab and make sure you are inside the Table structure subtab.
- Check the first_name column.
- Click the Change option.
- Uncheck the Null option.
- Click Save.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/10.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/10.2.png)
### Foreign keys: A foreign key is a column that establishes a relationship between two tables. It acts as a cross-reference between two tables as it points to the primary key of one table (the parent table), constraining the data in another table (the child table) by the data in the parent table. You will create a foreign key for the book_authors table by setting its author_id column as a foreign key, to establish a relationship between the book_authors and authors tables.

In the tree-view, click the book_authors table. Switch to the Structure tab and make sure you are inside the Relation view subtab.
- If necessary, click Add constraint to create a new foreign key constraint placeholder.
- Fill the placeholders as shown in a image below.
- Click Save.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/11.1.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/11.2.png)
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Keys%20and%20Constraints%20in%20MySQL/images/11.3.png)

CASCADE means that when rows are deleted or updated in the parent table, the corresponding rows in the child table will also be deleted or updated.

RESTRICT means that rows cannot be deleted or updated in the parent table if there are corresponding rows in the child table.
## After creating/adding all the above necessary primary keys, foreign keys, and constraints, the schema of the complete eBooks database
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/eBooks/eBooks_schema_complete.png)
