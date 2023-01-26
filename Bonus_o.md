<h2>Install a relational database, show CRUD operations using SQL</h2>

<h4> Disclaimer</h4>
I already had a MSQL Server Management Studio installed so can't showcase how I did it!

<h3>The data</h3>

i chose to put the whole script I created here so others can try it out:


<h4>Creating tables</h4>

I created 2 tables Student and DormRoom:

CREATE TABLE Student
(
	first_name VARCHAR(20) NOT NULL,
	last_name VARCHAR(2) NOT NULL,
	student_number VARCHAR(3) NOT NULL,
	gpa SMALLINT NOT NULL,
  CONSTRAINT PK_Student PRIMARY KEY (student_number),
)


CREATE TABLE DormRoom
(
	room_number SMALLINT NOT NULL,
	room_size VARCHAR(5),
	student_number VARCHAR(3) NOT NULL,
  CONSTRAINT PK_DormRoom PRIMARY KEY (room_number),
	CONSTRAINT FK_Student_DormRoom FOREIGN KEY (student_number) REFERENCES Student(student_number)
)


<h4>Inserts</h4>
I then inserted data to both tables:

INSERT INTO Student (first_name, last_name, student_number, gpa) VALUES
('Oskari', 'Ruotsalainen', 's11', 4),
('Petri', 'Ruotsalainen', 's12', 5),
('Veera', 'Ruotsalainen', 's13', 3),
('Timo', 'Ruotsalainen', 's14', 2)


INSERT INTO DormRoom (room_number, room_size, student_number) VALUES
(1, 'big', 's11'),
(2, 'small', 's12'),
(3, 'big', 's13'),
(4, 'small', 's14')

<h4>Selects</h4>
Selected all of the data to check that everything works:

SELECT * 
FROM Student;


SELECT *
FROM DormRoom;

<h4>Updates</h4>
Tested updates:

UPDATE Student
SET gpa = 5
WHERE student_number = 's11';


UPDATE DormRoom
SET room_size = 'big'
WHERE room_number = 4;

<h4>Deletes</h4>
Tested deletes:

DELETE FROM DormRoom WHERE room_number = 2;

DELETE FROM Student WHERE student_number = 's12';

<h5>Here's also a screenshot:<h5>


![SQL_Tables](https://user-images.githubusercontent.com/78789083/214944229-4fc936a7-0cc1-43bb-b7da-a29a613acf77.PNG)

  
 If a problem occurs run these commands to drop the tables and start over:
  
 ```
  DROP TABLE DormRoom
  DROP TABLE Student
  ```
  
  <h4>Selects results</h4>
  
  ![image](https://user-images.githubusercontent.com/78789083/214944626-35a3c3e4-10e8-422c-9aa1-a6d62f6b94e7.png)
  
  ![image](https://user-images.githubusercontent.com/78789083/214944706-791ac061-d278-4acd-927d-a6377e7cf615.png)

  <h4>Selects results after updates and deletes</h4>
  
  ![image](https://user-images.githubusercontent.com/78789083/214944858-20e59afe-1a61-4d68-b6b6-b200ba579160.png)

  ![image](https://user-images.githubusercontent.com/78789083/214944914-7bb919e3-40c6-4d0f-b5e3-a99331f36be2.png)

  
  
  
