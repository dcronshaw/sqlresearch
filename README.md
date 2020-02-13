# dbresearch


## Referential Integrity
  Referential integrity is a series of constraints that prevent your database from having null or invalid values. For example, if you tried to enter a value of "3" in your foreign key, and your primary key didn't have an id of "3", the foreign key would be rejected.
  
 
 ### Domain Constraints
  Domain constraints refer to the type of value allowed. For example, character, integer, date, ENUM, etc. These will reject any non allowed values. 
  
  
 ### Key Constraints
  Key constraints are used to identify columns and relate tables to each other. The usual key constraints are Primary, Foreign, and Unique. Primary keys are a unique value that defines each of the rows in any given table. Foreign keys are keys that are used to relate a row in a table to another table(the foreign key and primary key must have the same domain constraint). Unique keys are similar to primary keys, as they contain unique values. However, there can be only one primary key in each table, where unique keys can be plentiful, and can be entered with a null value.
  
### Referential Integrity Constraints
  Referential integrity constraints refer to the relationships between two entities(tables, etc). This states that they must share domain constraints, and values.
  

## ER Diagrams
  ER(entity relational) diagrams are used to show how the database will be set up, and the relationships between the entities, with all of the keys illustrated in an easy to read, well laid out format. ERDs also allow you to better visualize the flow of your database, and neatly shows the relationships between entities.  
  
## Data Normalization
  Data normalization is a process used to significantly reduce or eliminate redundancies in databases. This forces the database to have information in one place only, therefore eliminating inconsistencies between entities. 
  
### 1NF
  1NF(first normal form) requires the elimination of repeating groups in individual tables by grouping data by relations, and giving them an identifier(primary key).
  
### 2NF
  2NF(second normal form) requires each value to be declared if one table only, and then provided to others using foreign keys. For example, if you're running an Ecommerce site, Customer Name is probably requrie by billing, shipping, etc, but may only be declared in the customer table. 
  
### 3NF
  3NF(third normal form) require the elimination of any values that are not directly related to the primary key in a table.
This can be achieved by creating new tables for the unrelated values, and linking them in using foreign keys.  *note* Using 3NF is not entirely practical. By using lots of different tables, it can significantly slow down the speed and efficiency of your database.
  
## Indexes
  Indexes are used to speed up searches by grouping together columns. For example, if you had two columns, first_name and last_name, you could make an index called full_name(or something to this effect) combining them into one. Indexes are unable to be seen by the end user, they are strictly there to speed up the database queries.
  
## Relational vs Non-relational Databases
  The main difference between relational and non-relational databases, is the presence or lack of strict constraints and structure. 
  
### Relational
  Relational databases should be used if you have a strict structure and layout you are planning on using. If you are planning on pushing and pulling data from the database regularly, your structure is not going to change, and want to easily query, relational is definitely the way to go for you.
  
### Non-relational
  Non-relational is perfect if you're developing an app, and need to store large amounts of data. It is much easier to change on the fly, and will not get you bogged down with restrictions. 
  
  
## PHP or MYSQL
  According to the experts, doing work on the db side should be avoided if possible, to prevent changing or deleting important data. There are some exceptions however. Deleting or reducing data should be done by mysql, as should sub-queries and joins. 
  
  




