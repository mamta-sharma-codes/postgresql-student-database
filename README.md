# postgresql-student-database
Student Database Management Project using PostgreSQL
CREATE TABLE students (
    student_id INT PRIMARY KEY,
    student_name VARCHAR(100),
    age INT,
    city VARCHAR(50)
);

INSERT INTO students
(student_id, student_name, age, city)
VALUES
(1, 'Rahul', 21, 'Pune'),
(2, 'Priya', 22, 'Mumbai'),
(3, 'Amit', 20, 'Delhi');

-- Display all students
SELECT * FROM students;

-- Display students older than 20
SELECT *
FROM students
WHERE age > 20;

-- Display students in Pune
SELECT *
FROM students
WHERE city = 'Pune';

-- Count the total number of students
SELECT COUNT(*)
FROM students;
