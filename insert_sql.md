Dumping data for table Student

INSERT INTO Student (Student id, name, Phone, age, address), VALUES (
1233, poojeetha, 9640525427, 23, {hyderabad, karmanghat} ), (1234,
 vineeth, 9640527893, 25, {hyderabad, madinaguda}), (3122,
matrupally, 9392103716, 26, {jntu, hyderbad}), (4211, vidharth,
8309561236, 16, nizambad), (5612, Abdul, 8309561258, 32,
parkal);

Dumping data for table Courses

INSERT INTO courses (id (Student_id), name, instructor, department),
VALUES (1,  poojeetha, rakshitha,  mech), ( 2,  vineeth, 
vishnupriya,  datascience), 3,  matrupally,  venkatesh, CSC ),
(4,  vidharth,  Ahmed,  EEE), ( 5,  Abdul,  Vikas,  BA)

Dumping data for table Instructors

INSERT INTO Instructors (id, name, email, office), VALUES (1233,
rakshitha, rakshitha@gmail.com, Amazon), (3122, venkatesh,
venkatmadugula@gmail.com, TechM), (1234, vishnupriya,
venvishnupriya@gmail.com, Amazon), (4211, Ahmed,
Ahmed@gmail.com, TechM), (5612, vikas, vmatrupa@gmail.com,
virtusa)

Dumping data for table enrollments

INSERT INTO enrollments (id, Student_id, course_id, grade), VALUES
(123456, 1233, 2, A), (223456, 1234, 1, A), (346245, 4211, 4, B),
(545361, 3122, 3, C), (776563, 6612, 5, F)
