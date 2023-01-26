<h2>Joins</h2>

Created two select to demonstrate joins:

```
SELECT last_name, first_name, Student.student_number, room_number
FROM Student
JOIN DormRoom ON (Student.student_number = DormRoom.student_number);

SELECT room_size, last_name, room_number
FROM DormRoom
JOIN Student ON (Student.student_number = DormRoom.student_number);
```

<h3>Results</h3>


1.

![image](https://user-images.githubusercontent.com/78789083/214951746-349977c9-d0d0-4859-9e5c-06c212c655b1.png)

2.

![image](https://user-images.githubusercontent.com/78789083/214951829-f9b33ddb-b804-481d-87ca-0ae3f98cec9a.png)

On both the tables data is joined by using the foreign key of student_number on DormRoom and primary key student_number on Student.


(The select value Student.student_number needs to be written so, because both tables have the value student_number)

