SELECT * FROM students;

SELECT * FROM courses;

SELECT * FROM instructors;

SELECT * FROM enrollments;





-- 
-- Dumping data for table 'students'
--

INSERT INTO students (id, name, phone, age, address)
VALUES (1, 'John Doe', '555-123-4567', 18, '123 Main Street'),
       (2, 'Jane Smith', '555-555-5555', 20, '456 Elm Street'),
       (3, 'Bob Johnson', '555-987-6543', 19, '789 Oak Avenue'),
       (4, 'Sarah Lee', '555-555-1212', 21, '321 Maple Drive'),
       (5, 'Tom Jones', '555-444-3333', 22, '654 Pine Street Apt. 2B');


-- -------------------------------------------------------------
-- 
-- Dumping data for table 'courses'
--

INSERT INTO courses (id, name, instructor, department)
VALUES (1, 'Introduction to Physics', 'Dr. Smith', 'Physics'),
       (2, 'Calculus I', 'Prof. Johnson', 'Mathematics'),
       (3, 'Intro to Computer Science', 'Prof. Lee', 'Computer Science'),
       (4, 'American Literature', 'Dr. Brown', 'English'),
       (5, 'Organic Chemistry', 'Prof. Kim', 'Chemistry');


-- 
-- Dumping data for table 'instructors'
--

INSERT INTO instructors (id, name, email, office)
VALUES (1, 'Dr. Smith', 'drsmith@university.edu', 'Science Building, Room 101'),
       (2, 'Prof. Johnson', 'pjohnson@university.edu', 'Math Building, Room 203'),
       (3, 'Prof. Lee', 'plee@university.edu', 'Computer Science Building, Room 304'),
       (4, 'Dr. Brown', 'dbrown@university.edu', 'Humanities Building, Room 102'),
       (5, 'Prof. Kim', 'pkim@university.edu', 'Science Building, Room 205');


-- 
-- Dumping data for table 'enrollments'
--

CREATE TABLE enrollment (
    id INT PRIMARY KEY,
    student_id INT,
    course_id INT,
    grade INT
);

INSERT INTO enrollment (id, student_id, course_id, grade)
VALUES (1, 101, 1, 90),
       (2, 102, 2, 85),
       (3, 103, 1, 95),
       (4, 104, 3, 80),
       (5, 105, 4, 92);


delete from students where id=1;

delete from courses where id=1;

delete from instructors where id=2;

delete from emrollment where id=2;


ALTER TABLE 'students'
    ADD PRIMARY KEY ('id'),

ALTER TABLE 'courses'
    ADD PRIMARY KEY ('id'),

ALTER TABLE 'instructors'
    ADD PRIMARY KEY ('id'),

ALTER TABLE 'enrollments'
    ADD PRIMARY KEY ('id'),

ALTER TABLE 'students'
    MODIFY 'id';

ALTER TABLE 'courses'
    MODIFY 'id';

ALTER TABLE 'instructors'
    MODIFY 'id';

ALTER TABLE 'enrollments'
    MODIFY 'id';

