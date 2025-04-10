##  Quantitative Assessment Summary

| Evaluation Criteria | Implementation | Grade Level |
|---------------------|----------------|-------------|
| **Environment** | Deployed on Vercel (Frontend) and Render or Railway (Backend) | Grade 5 |
| **Backend** | Developed using Node.js with Express.js | Grade 5 |
| **Frontend** | Built using React.js and styled with Bootstrap | Grade 5 |
| **Database** | Using PostgreSQL via Prisma ORM | Grade 5 |

---

##  Qualitative Assessment

###  Basic Structure and Architecture – Grade 5

#### Architecture Overview
- **Frontend:** React.js SPA (Single Page Application)
- **Backend:** RESTful API with Express.js
- **Database:** PostgreSQL
- **NFC Integration:** Web NFC API simulation (for development) or physical NFC reader
- **Documentation:**  
  - `README.md` includes setup instructions, stack overview, and architecture diagram  
  - All major components, routes, and data flows are diagrammed and commented

---

###  Functionalities – Grade 5

| Feature | Implemented? | Notes |
|--------|--------------|-------|
| Teacher Course Creation |  | Teachers can create new courses with title, code, and description |
| Session Scheduling |  | Sessions are linked to courses with date/time |
| NFC Student Tap-in |  | NFC ID and timestamp are recorded to the database |
| Automated Hours Calculation |  | Duration calculated based on session start/end and attendance tap time |
| Attendance History |  | Teachers can view per-course attendance logs |
| Real-time Updates |  | WebSocket or polling updates attendance view in real-time |

---

###  Code Quality and Documentation – Grade 5

- Follows a clear folder structure: `/components`, `/routes`, `/services`, etc.
- Inline comments are present to explain logic in modules
- ESLint enforces code style; Prettier used for consistent formatting

Below are some screenshots showcasing the API endpoints and functionalities.

### Endpoints Screenshot 1
<img src="StuAttendanceAPI/StuAttendanceAPI.WebApi/Documentation/endpointsscreenshot.jpg" alt="Endpoints Screenshot 1"/>

### Endpoints Screenshot 2
<img src="StuAttendanceAPI/StuAttendanceAPI.WebApi/Documentation/endpointsscreenshot2.jpg" alt="Endpoints Screenshot 2"/>

### Endpoints Screenshot 3
<img src="StuAttendanceAPI/StuAttendanceAPI.WebApi/Documentation/endpointsscreenshot3.jpg" alt="Endpoints Screenshot 3"/>

## API Endpoints

Below are the detailed API endpoints available in the StuAttendanceAPI.

### Students

- **GET** `/students`  
  Retrieve all students.

- **GET** `/students/{id}`  
  Retrieve a student by ID.

  - **POST** `/students`  
  Create a new student.

- **PUT** `/students/{id}`  
  Update an existing student.

- **DELETE** `/students/{id}`  
  Delete a student.

### Attendance

- **GET** `/attendance`  
  Retrieve all attendance records.

  - **GET** `/attendance/{id}`  
  Retrieve an attendance record by ID.

- **GET** `/attendance/student/{studentId}`  
  Retrieve attendance records for a specific student.

- **POST** `/attendance`  
  Create a new attendance record.

- **PUT** `/attendance/{id}`  
  Update an existing attendance record.

- **DELETE** `/attendance/{id}`

  ### Course

- **GET** `/api/Course`  
  Retrieve all courses.

- **GET** `/api/Course/{id}`  
  Retrieve a course by ID.

- **POST** `/api/Course`  
  Create a new course.

- **PUT** `/api/Course/{id}`  
  Update an existing course.

  - **DELETE** `/api/Course/{id}`  
  Delete a course.

- **GET** `/api/Course/GetCoursesByStudentId/{studentId}`  
  Retrieve courses by student ID.

### Session

- **GET** `/api/Session`  
  Retrieve all sessions.

- **GET** `/api/Session/{id}`  
  Retrieve a session by ID.
- **POST** `/api/Session`  
  Create a new session.

- **PUT** `/api/Session/{id}`  
  Update an existing session.

- **DELETE** `/api/Session/{id}`  
  Delete a session.

- **GET** `/api/Session/GetSessionsByCourseId/{courseId}`  
  Retrieve sessions by course ID.

  ### User

- **GET** `/api/User`  
  Retrieve all users.

- **GET** `/api/User/{id}`  
  Retrieve a user by ID.

- **POST** `/api/User`  
  Create a new user.

- **PUT** `/api/User/{id}`  
  Update an existing user.

  - **DELETE** `/api/User/{id}`  
  Delete a user.

- **POST** `/api/User/Login`  
  User login.

     
