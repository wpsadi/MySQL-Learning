# Creating Table / 1.

CREATE Table Training(
    Training_Id char(4) PRIMARY KEY,
    Name varchar(255) NOT NULL,
    Email_Id varchar(255) UNIQUE,
    Topic varchar(255), 
    City varchar(255) DEFAULT "Faridabad",
    Fee INT
)

# Entering values / 2.
INSERT INTO Training VALUES("ND01","Mr. Ranjan","raj@gmail.com","Cyber Security","New Delhi",10000);

INSERT INTO Training VALUES("GU01","Ms. Urvashi","urv@yahoo.com","ICT in Education","Gurugram",15000);

INSERT INTO Training VALUES("FD01","Ms. Neena","neenarediff.com","Cyber Security","Faridabad",12000);

INSERT INTO Training(Training_Id,Name,Topic,City,Fee) VALUES("ND02","Mr. Vinay","ICT in Education","New Delhi",13000);

INSERT INTO Training(Training_Id,Name,Email_id,Topic,City) VALUES("GU02","Mr. Naveen","nav@gmail.com","Cyber Security","Gurugram");


# Display Records / 3.
SELECT * FROM Training;

# Display Specific Attributes / 4.
SELECT Name,Email_Id,Fee FROM Training;