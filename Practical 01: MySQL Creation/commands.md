# Creating Table / 1.

CREATE Table Training(
    Training_Id char(4) PRIMARY KEY,
    Name varchar(255) NOT NULL,
    Email_Id varchar(255) UNIQUE,
    Topic varchar(255), 
    City varchar(255) DEFAULT "Faridabad"
)