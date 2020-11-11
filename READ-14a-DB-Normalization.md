# Database Normalization

- A process used to organize a database into tables and columns.

- The main idea with this is that a table should be about a specific topic and only supporting topics included.

- By limiting a table to one purpose you reduce the number of duplicate data contained within your database.

- There are three main reasons to normalize a database.  

1. To minimize duplicate data.

2. To minimize or avoid data modification issues. 

3. To simplify queries. 

- There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. 

`First Normal Form` – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.

`Second Normal Form` – The table is in first normal form and all the columns depend on the table’s primary key.

`Third Normal Form` – the table is in second normal form and all of its columns are not transitively dependent on the primary key