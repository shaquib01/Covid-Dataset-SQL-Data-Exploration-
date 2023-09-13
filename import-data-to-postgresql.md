# Import excel data to postgre sql 
This is the instruction for the importing data to postgre SQL 


## Before, exporting data, first you have to create a table name "covid-death"
 - You can creating by just navigation to public ,Then in Schema Tables 
 - Right Click, create a Table
 or you can run Query :
  ```
  create table "table name"
  (
    column_name1 type,
    column_name2 type
  );
  ```

## Importing data 

```
COPY covid_death (columnname_1,column_name2)
from "path:/customer_vaccination.csv"
Delimiter ','
CSV HEADER ;
```
(locate the local directory of your file)

## But the fact is there is lots of column in the dataset , adding column name manually is bit difficult 

- at first , i openmy csv file through notepad and copy all the column name and add their data type manually 
- but it bigcome bit difficult , and my data is not sucessfully imported
- some column has 'bigint' data type  so 

then i  alter table data type: 
 - still, it did not get succeed !

 # Then I will try in next day ! stay tunned :)