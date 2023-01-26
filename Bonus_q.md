<h2>Aggregate functions</h2>

this thas was simple, I used the following commands:

```
SELECT SUM(GPA)
FROM Student;

SELECT SUM(room_number)
FROM DormRoom;

SELECT COUNT(student_number) AS 'Student amount'
FROM Student;

SELECT COUNT(room_number) AS 'Amount of rooms'
FROM DormRoom;

```

1. Student GPAs summed: 14
2. Room numbers summed: 10
3. Students counted: 4
4. Rooms counted: 4

Here's also a screenshot of the commands:

![image](https://user-images.githubusercontent.com/78789083/214950528-78c9541e-c07f-4e8e-804a-669b7066f660.png)

Also some bonus ones I did:

```
SELECT AVG(GPA)
FROM Student;

SELECT MAX(room_number)
FROM DormRoom;

SELECT MIN(GPA)
FROM Student;
```

1. Shows GPA average: 3
2. Shows biggest room number: 4
3. Shows smallest GPA: 2
