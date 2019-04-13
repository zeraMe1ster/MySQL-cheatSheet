 MySQL-cheatSheet

===============

Commands
-----------

Initial command: mysql -u root -p 

Show all database from the system : show databases;

Create new database: create database thisWillBeDataBaseName;

Select database: use enterTheNameOfDB;

Create table : create table nameYourTable;

Adding a column: ALTER TABLE [tableName] ADD COLUMN [columnName] datatype;

Set up PK and features : ALTER TABLE [tableName] ADD COLUMN [newColumnName] int NOT NULL AUTO_INCREMENT PRIMARY KEY;`

Tables View: show tables;

Table structure: describe tableName;

List all indexes of a table: show index from tableName;

Insert a record: INSERT INTO [table] ([column], [column]) VALUES ('[value]', [value]');

MySQL function for datetime input: NOW()

Selecting records: SELECT * FROM [table];

Updating records: UPDATE [table] SET [column] = '[updated-value]' WHERE [column] = [value];

Deleting records: DELETE FROM [table] WHERE [column] = [value];

Delete all records in a table: truncate table [table];

Removing table columns: ALTER TABLE [table] DROP COLUMN [column];

Deleting tables: DROP TABLE [table];

Deleting databases: DROP DATABASE [databaseName];

Logout: exit;




Users functions
-----------

List mysql users: SELECT User,Host FROM mysql.user;

Create new user: CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';

Grant `ALL` access to user for `*` tables: GRANT ALL ON database.* TO 'user'@'localhost';

