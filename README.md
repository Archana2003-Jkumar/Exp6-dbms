# Exp6-dbms
# SET OPERATIONS
## AIM:
The aim of this program is to perform set operations (Union, Union All, Intersect, and Except) between two tables, A and B, in order to combine, find common elements, or identify differences between the tables.

## ALGORITHM:
1.Create table A with attributes ID and name.

2.Create table B with attributes ID and name.

3.Insert values into table A.

4.Insert values into table B.

5.Display the contents of table A.

6.Display the contents of table B.

7.Perform set operations: a. Union: Combine rows from table A and table B, eliminating duplicates. b. Union All: Combine rows from table A and table B, including duplicates. c. Intersect: Find common rows between table A and table B. d. Except: Find rows in table A that do not exist in table B.

8.Display the results of each set operation.
## PROGRAM:
```
create database if not exists MyDatabase;
use MyDatabase;
CREATE TABLE A (
  ID INTEGER PRIMARY KEY,
  name TEXT
);

CREATE TABLE B (
  ID INTEGER PRIMARY KEY,
  name TEXT
);

-- Insert values into table A
INSERT INTO A VALUES (1, 'John');
INSERT INTO A VALUES (2, 'Alice');
INSERT INTO A VALUES (3, 'Bob');

-- Insert values into table B
INSERT INTO B VALUES (2, 'Alice');
INSERT INTO B VALUES (3, 'Bob');
INSERT INTO B VALUES (4, 'Charlie');

-- Display table A
SELECT * FROM A;

-- Display table B
SELECT * FROM B;

SELECT * FROM A
UNION
SELECT * FROM B;

SELECT * FROM A
UNION ALL
SELECT * FROM B;

SELECT * FROM A
INSERTSET;
SELECT * FROM B;

SELECT * FROM A
EXCEPT
SELECT * FROM B;
```
## OUTPUT:
### The output for table A will be:
![image](https://github.com/Archana2003-Jkumar/Exp6-dbms/assets/93427594/8389008a-2ec3-4624-a517-963f19c6c21e)

### The output for table B will be:
![image](https://github.com/Archana2003-Jkumar/Exp6-dbms/assets/93427594/4b66492c-5740-481a-b27b-e5e6f6c1c826)
### Union:
![image](https://github.com/Archana2003-Jkumar/Exp6-dbms/assets/93427594/14bd4147-d2b8-4bfb-8730-1d13204feb0b)
### Union All:
![image](https://github.com/Archana2003-Jkumar/Exp6-dbms/assets/93427594/a4e16bc9-e02f-49d1-9dda-dac7772d1c61)
### Intersect:
![image](https://github.com/Archana2003-Jkumar/Exp6-dbms/assets/93427594/7065b5be-1175-4ec4-a1b8-382386843a19)
### Except:
![image](https://github.com/Archana2003-Jkumar/Exp6-dbms/assets/93427594/dc227a78-715c-4a68-884d-1b2419ed2664)
### RESULT:
These results illustrate the outcomes of the set operations performed on tables A and B.

