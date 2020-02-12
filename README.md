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


