# Rest_Server_Spring
## ***About project***

This is a simple Rest Server Spring app which work with entity Employee. Also as a Rest Client you can use project Rest_Client on my GitHub or Postman. Also you can use JSON viewer for your browser and use it for simple view data.

Base URL - http://localhost:8080/spring_course_rest/api

#### Endpoints:
/employees - method GET. Get all list Employees.
<br/> /employees/{id} - method GET. Get Employee by ID.
<br/> /employees - method POST or PUT. Use Body of HTTPRequest for save or Update Employee.
<br/> /employees/{id} - method DELETE. Delete Employee by ID.



## ***Configuration***

- Java 11
- Tomcat version 9.0.58
- MySQL Workbench:
    + **_DriverClass:_** com.mysql.cj.jdbc.Driver;
    + **_JdbcUrl:_** jdbc:mysql://localhost:3306/my_db?useSSL=false&serverTimezone=UTC&allowPublicKeyRetrieval=true;
    + **_User:_** bestuser;
    + **_Password:_** bestuser;


## ***Simple script for creating DataBase***

```
CREATE TABLE employees (
  id int NOT NULL AUTO_INCREMENT,
  name varchar(15),
  surname varchar(25),
  department varchar(20),
  salary int,
  PRIMARY KEY (id)
) ;

INSERT INTO my_db.employees (name, surname, department, salary)
VALUES
	('Zhanna', 'Tsarenko', 'IT', 500),
	('Oleg', 'Ivanov', 'Sales', 700),
        ('Dima', 'Kitchenko', 'Sales', 700),
        ('Olena', 'Timchenko', 'IT', 500),
	('Nina', 'Sidorova', 'HR', 850),
        ('Zina', 'Torenko', 'IT', 650),
	('Oksana', 'Ovcharenko', 'Sales', 700),
        ('Dima', 'Oleshiv', 'Sales', 700),
        ('Vadym', 'Cat', 'IT', 500),
	('Serg', 'Simchenko', 'HR', 850);
```
