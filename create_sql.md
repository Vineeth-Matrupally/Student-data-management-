--
-- Table structure for table 'students'
--

CREATE TABLE IF NOT EXISTS students(
                  id INTEGER PRIMARY KEY,
                  name TEXT,
                  phone TEXT,
                  age INTEGER,
                  address TEXT);


-- --------------------------------------------
--
-- Table structure for table 'courses'
--

CREATE TABLE IF NOT EXISTS courses(
                  id INTEGER PRIMARY KEY,
                  name TEXT,
                  instructor TEXT,
                  department TEXT,
                  FOREIGN KEY (instructor) REFERENCES instructors(name));


--
-- Table structure for table 'instructors'
--

CREATE TABLE IF NOT EXISTS instructors(
                  id INTEGER PRIMARY KEY,
                  name TEXT,
                  email TEXT,
                  office TEXT);


-- 
-- Table structure for table 'enrollments'
--

CREATE TABLE IF NOT EXISTS enrollments (
                  id INTEGER PRIMARY KEY,
                  student_id INTEGER,
                  course_id INTEGER,
                  grade TEXT,
                  FOREIGN KEY (student_id) REFERENCES students(id),
                  FOREIGN KEY (course_id) REFERENCES courses(id));

--
