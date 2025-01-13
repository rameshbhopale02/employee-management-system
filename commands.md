## SQL IMPLMENTATION
1. Start server - mysql -u root -p
2. Create database - create database employees;
3. Change database - use employees;
4. Create table - create table employeeDetails (id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(255) NOT NULL, dateOfBirth DATE, joiningDate DATE, salary DECIMAL(10, 2), department VARCHAR(255));
5. Describe table - describe employeedetails;
6. Insert into table - INSERT INTO employeedetails (name, dateOfBirth, joiningDate, salary) VALUES ("Example Name", "2004-02-27", "2023-11-01", 5000.00);
7. delete query :-
   -  DELETE FROM employeedetails
   -  WHERE
   - id = XYZ
   - name = "XYZ"
   - joiningDate = "XX-YY-ZZZZ"
   - birthdate = "XX-YY-ZZZZ"
   - salary = XYZ

9. seach Query :- SELECT * FROM employeedetails where {id , name, joiningdate, birthdate, salary) 
10. update query :- update employeedetails set id = 123, name='ram', joiningdate = 'xx-yy-zzzz' where {id, salary, name, joiningdate, birthdate}
11. get all employee :- select * from employeeDetails
12.   
   
    



