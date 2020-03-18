# SQL 
________

- Is a language that allows both technical and non technial users manipulate and transform data from a relational database.
- Relational Databases are 2 dimensional tables where the columns are number that represent attributes or properties and the rows are the data.
- A query is a select statement that looks for data , what database it is in and  how we want to change it before it returns . Looks like the following 
```
Select query for a specific columns
SELECT column, another_column, … ( you can put( SELECT * ) TO SELECT ALL THE COLUMNS)
FROM mytable;
```

- Here are some of the logical operators :-
Operator	|Condition|SQL Example
________________________________________
=, !=, < <=, >, >=	|Standard numerical operators	|col_name != 4
BETWEEN … AND …	Number |is within range of two values (inclusive)	|col_name BETWEEN 1.5 AND 10.5
NOT BETWEEN … AND …	Number| is not within range of two values (inclusive)|	col_name NOT BETWEEN 1 AND 10
IN (…)	|Number exists in a list	|col_name IN (2, 4, 6)
NOT IN (…)	|Number does not exist in a list	|col_name NOT IN (1, 3, 5)

- To insert rows of data as well as specify what column yo want it to go.
- Spaces are not used and the code will not write so you use commas instead
``` 
INSERT INTO mytable
(column, another_column, …)
VALUES (value_or_expr, another_value_or_expr, …),
      (value_or_expr_2, another_value_or_expr_2, …),
      …;
``` 
TO delete a row :
``` 
Delete statement with condition
DELETE FROM mytable
WHERE condition;
``` 


- To create a table :
```
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);
```