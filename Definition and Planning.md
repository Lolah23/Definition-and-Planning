### **Phase 1: Definition and Planning for TAPIN**  

#### **1. User Personas**  
- **Teacher (Primary User)**  
  - Age: 30–50  
  - Tech-savvy level: Moderate  
  - Goals: Create courses, track attendance, and monitor student participation.  
  - Pain Points: Difficulty tracking attendance manually, managing large classes, and ensuring accurate records.  
   
- **Student (Primary User)**  
  - Age: 16–25  
  - Tech-savvy level: High  
  - Goals: Quickly mark attendance using an NFC card, check attendance records, and avoid missing classes.  
  - Pain Points: Forgetting to sign attendance, long manual processes, and lack of instant feedback.  
   
- **Administrator (Secondary User)**  
  - Age: 25–40  
  - Tech-savvy level: High  
  - Goals: Manage the system, ensure NFC device functionality, and oversee attendance reports.  
  - Pain Points: Handling technical issues and maintaining security.  

#### **2. Use Cases and Usage Scenarios**  
- **Use Case 1: Teacher Creates a Course and Session**  
  - **Actor:** Teacher  
  - **Steps:**  
    1. Logs into TAPIN.  
    2. Creates a new course with a name, schedule, and session details.  
    3. Saves course, which becomes available for students.  

- **Use Case 2: Student Marks Attendance**  
  - **Actor:** Student  
  - **Steps:**  
    1. Taps NFC card on the device.  
    2. TAPIN verifies identity and records the timestamp.  
    3. Attendance status updates in real time.  

- **Use Case 3: Teacher Views Attendance Records**  
  - **Actor:** Teacher  
  - **Steps:**  
    1. Logs into TAPIN.  
    2. Selects a course and views attendance history.  
    3. Downloads attendance reports if needed.  

- **Use Case 4: Administrator Manages System**  
  - **Actor:** Administrator  
  - **Steps:**  
    1. Logs in with admin privileges.  
    2. Adds or removes courses, teachers, or students.  
    3. Troubleshoots any system issues.  

#### **3. UI Prototypes**  
- **Teacher Dashboard:** Course creation form, session scheduling, attendance reports.  
- **Student Dashboard:** Attendance status, past attendance records.  
- **NFC Attendance Page:** Simple confirmation screen after tap-in.  
- **Admin Panel:** User management, system logs, and troubleshooting tools.  

#### **4. Information Architecture and Technical Design**  
- **Frontend:** React with Bootstrap for UI.  
- **Backend:** Node.js with Express.js for API endpoints.  
- **Database:** MongoDB (NoSQL) or PostgreSQL (SQL) for storing attendance records.  
- **NFC Integration:** JavaScript-based API for handling NFC card reads.  
- **Authentication:** JWT-based login system.  
- **Deployment:** Hosted on a cloud service (e.g., Vercel, Firebase, or AWS).  

#### **5. Project Management and User Testing**  
- **Development Methodology:** Agile (Scrum)  
- **Project Timeline:**  
  - **Phase 1:** Planning (2 weeks)  
  - **Phase 2:** Backend & Database Setup (3 weeks)  
  - **Phase 3:** Frontend Development (3 weeks)  
  - **Phase 4:** NFC Integration & Testing (2 weeks)  
  - **Phase 5:** Deployment & Final Testing (2 weeks)  

- **User Testing Plan:**  
  - **Unit Testing:** Each feature tested individually.  
  - **Integration Testing:** Testing NFC with the database.  
  - **Beta Testing:** Selected teachers and students provide feedback.  
  - **Final Release:** After improvements based on feedback.  
