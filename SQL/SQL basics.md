DBs are systems that allows users to store and organize data. Used to deal with large amount of data. 
There are different types of DBs: relation, non-relation, cloud, distributed.
The most used are relation and non-relation DBs. 
Relation DB stores data in tables. It is good for structured data and when relation matters. Like for stores, social medias, e-commerce. 
Non-relation DBs do not have relation and do not store data in tables. They store in sort of separate data documents like a plain text where you can pretty flexible change data as you want. 

**Example** for a store it can be used RDB you will have a structured data like users, items, orders, categories and so on. Meaning each table will be somehow connected with another tables. 
But in the same time with NRDB you can store user orders info in one "folder" for this user. When you open user with ID 72 John Smith it will show you all hs info + all his orders. Instead of connecting multiple tables in RDB to fetch data that is correlated with this user. 

**PROS & CONS**
For RDB are concistency, structure, relations and integrety. Harder to to change data often in a big DBs, hard to scale horizontally (its doable, just not easy to), and with scaling queries became more complex too.
For NRDB main aspect is flexability, meaning you can set data files structure as you want. But again no relations or structure, and badly handles duplicates.

So we will be working with RDB at least for now this is the only experience we have. To better understand the structure of a RDB table we need to know Primary key and Foreign key. 
**PK** - is a column that uniquely identifies each row in a table.There are some rules for a PK: it must be unique, cannot be NULL, should not change, identifies 1 exact row.
A **Foreign Key** is a column that connects one table to another table.
**NULL** - means that value is not provided. It is not a Zero, for example in a user table if customer does not provide a phone number it will be a NULL. 

