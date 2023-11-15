CREATE TABLE STUDENT(
    admno INT PRIMARY KEY,
    Name varchar(255) UNIQUE,
    fees INT,
    email varchar(255),
    city varchar(255),
    marks INT,
    DOB DATE
);

INSERT INTO STUDENT VALUES(101,'Anu',4000,'anu@gmail.com','UP',98,'2005-08-27');

INSERT INTO STUDENT(admno,Name,fees,DOB) VALUES(102,'Tanuj',1000,'2007-02-18');

INSERT INTO STUDENT(admno,Name,fees,email,city,marks) VALUES(103,'Tina',2000,'tina@hotmail.com','Delhi',72);

INSERT INTO STUDENT(admno,Name,fees,city,marks,DOB) VALUES(104,'Veena',1000,'UP',88,'2005-06-19');

SELECT * FROM STUDENT;

SELECT Name,fees,0.02*fees as discount_in_fees FROM STUDENT;

SELECT * FROM STUDENT WHERE fees<1500;

SELECT * FROM STUDENT WHERE (marks > 80) and;

SELECT * FROM STUDENT WHERE (marks > 80) AND (city = "UP");

SELECT * FROM STUDENT WHERE (city != "Delhi");

SELECT Name,fees,marks FROM STUDENT WHERE (DOB < "2007-01-01");

SELECT DISTINCT(city) FROM STUDENT;

SELECT * FROM STUDENT WHERE marks in (78,88,92);