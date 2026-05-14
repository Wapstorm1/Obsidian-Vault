DBs are systems that allows users to store and organize data. Used to deal with large amount of data. 
There are different types of DBs: relation, non-relation, cloud, distributed.
The most used are relation and non-relation DBs. 
Relation DB stores data in tables. It is good for structured data and when relation matters. Like for stores, social medias, e-commerce. 
Non-relation DBs do not have relation and do not store data in tables. They store in sort of separate data documents like a plain text where you can pretty flexible change data as you want. 

**Example** for a store it can be used RDB you will have a structured data like users, items, orders, categories and so on. Meaning each table will be somehow connected with another tables. 
But in the same time with NRDB you can store user orders info in one "folder" for this user. When you open user with ID 72 John Smith it will show you all hs info + all his orders. Instead of connecting multiple tables in RDB to fetch data that is correlated with this user. 

**PROS & CONS**
For RDB are concistency, structure, relations and integrety. Harder to to change data often in a big DBs, 