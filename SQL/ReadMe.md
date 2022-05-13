# Insert Data into Table:
Synatx:

```SQL
Insert Into <Table_Name>(Column1,column2....Column(n)) Values (Value1,Value2,Value3.....value(n))
```

Example:
```SQL
INSERT INTO Student(Roll,Name,Address,Gender,Total_Fee) VALUES (1,'Pharping','M',20000)
```
# To View Distinct Data we use DISTINCT keyword:
Syntax:
``` SQL
INSERT DISTINCT COLUMN_NAME FROM TABLE_NAME;
```

Example:
```SQL
INSERT DISTINCT Adress FROM Student;
```

# To Delete Data from Table:
Synatx:
```SQL
DELETE FROM <TABLE_NAME> WHERE CONDITION
```
Example:
```SQL
DELETE FROM Student WHERE id=1;
```

# Update Data from Table:
Syntax:
```SQL
UPDATE <Table_name> SET Column_name = Value WHERE Condition 
```
Example:
```SQL
UPDATE Student Gender = "F" WHERE roll=1;
```

# WHERE CLAUSE
Syntax:
```SQL
SELECT  * FROM <Table_Name> WHERE Condition
```

Example:
```SQL
SELECT * FROM Student WHERE Gender = "M";
```

# AND :
Syntax:
```SQL
SELECT * FROM <Table_Name> WHERE Condition1 and Condition and....
```

Example:
```SQL
SELECT * FROM Student WHERE GENDER = "M" AND Total_fee=2000
```

# IN
Syntax:
```SQL
SELECT * FROM <Table_Name> WHERE Column_Name IN(Values,values)
```

Example:
```SQL
SELECT * FROM Student WHERE Adress IN ("Lalitpur","Kathmandu")
```

# NOT IN
Syntax:
```SQL
SELECT * FROM <Table_Name> WHERE Column_Name NOT IN(Values,values)
```

Example:
```SQL
SELECT * FROM Student WHERE Adress NOT IN ("Lalitpur","Kathmandu")
```

# NULL and EMPTY:
* NULL is Nothing. 
* Empty is defined as the  value with zero length.

# ORDER CLAUSE:
Order Table according to condtion in acending or decending order.

Syntax:
```SQL
SELECT * FROM <Table_Name> ORDER BY Column
```

EXample:
```SQL
SELECT * FROM Student ORDER BY ROLL 
```

# MIN,MAX,AVG:
```SQL
SELECT MIN(Column_Name) FROM TABLE_NAME;
SELECT MAX(Column_Name) FROM TABLE_NAME;
SELECT AVG(Column_Name) FROM TABLE_NAME;
```

# LIKE OPERATOR:
It helps to search the data.

### Wildcard:
*  % It represent any Text
    * SELECT * FROM Student WHERE Name Like '%a'.
  
      =>It will select all name start with A from start.

    * SELECT * FROM Student WHERE Name like 'a%'.
  
      =>It will select all name start from a from end.

    * SELECT * FROM Student WHERE Name Like "%ad";
   
      =>It will select all name which have word ad Consecutive.
      
     
b. _ It represent single Character.


