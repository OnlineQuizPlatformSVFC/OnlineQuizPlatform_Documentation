## A. Introduction
The online quiz platform aims to provide a simple digital solution for teachers to create, manage and distribute quizzes to students. The platform allows students to take online quizzes, receive instant feedback and track their progress. The goal is to enhance the learning experience by providing a flexible and interactive environment for teachers and students. The system will also simplify grading, reduce paper usage, and facilitate classification of quiz materials.


## B. Project Features and Characteristics
     • Quiz Creation Tool: Create quizzes with various question types, including multiple choice, true/false, short answer, and multimedia-enhanced questions.
     
       User Roles and Permissions: Separate dashboards and functionalities for teachers (quiz creation, grading, analytics) and students (taking quizzes, viewing 
       results).
       
       Analytics and Reporting: Provides performance data, quiz statistics, and insights into student progress.
       
       Mobile Responsiveness: The platform adapts to mobile devices, ensuring a seamless experience across desktops and smartphones.
       
       User-Friendly Interface: Intuitive design for both teachers and students, making the platform easy to navigate.
       
       Scalability: Capable of handling a large number of users, with support for future expansion.
       
       Customizability: Teachers can customize quizzes, question formats, and assign quizzes to different student groups.
       
       Accessibility: Designed with accessibility in mind, following guidelines to support users with disabilities.
       
       Documentation and Training: Comprehensive user guides, training materials, and thorough testing to ensure a smooth onboarding and usage experience.


## C. Project Scope
    • The Online Quiz Platform is a web application created to make it easier to create, administer, and take part in online quizzes. With a tools for making and   
      administering quizzes, taking quizzes, getting feedback, and analyzing outcomes, this platform will serve both administrators and users to security measures, 
      an intuitive user interface, and an adaptable question management system that supports a range of question kinds and difficulty levels will all be features of 
      the platform.
      The platform will also be made to be universally accessible, adaptable, and responsive to mobile devices. A working web application, thorough documentation, 
      extensive testing, and training materials to guarantee successful implementation and usage are all part of the project deliverables.
      
    • The online quiz platform may face limitations in customization for complex quiz formats and handling large user loads, which could impact performance. Security challenges such as preventing 
      cheating and data breaches could affect reliability. Limited offline functionality means users need a stable internet connection, restricting access in areas with poor connectivity.
     

## D. Work breakdown Structure
The main actions involved in creating an online quiz platform are delineated in this Work Breakdown Structure (WBS). The project is divided into manageable parts by it's hierarchical structure.

![image](https://github.com/user-attachments/assets/11518cf3-96cd-4585-b922-61b2a4ba4dee)


## E. Functional Requirements

        1. User  Requirements
| No. |                 | System Features                                           | Requirement                                                                 |
|-----|-------------------------|-----------------------------------------------------------|------------------------------------------------------------------------------|
| 1   |  Admin   | A. Quiz Management                                        | 1. Ability to create and customize quizzes with different types of questions (multiple-choice, true/false, short answer, essay). |
|     |                         |                                                           | 2. Capability to schedule quizzes for specific dates and times.              |
|     |                         |                                                           | 3. Option to set time limits for each quiz.                                   |
|     |                         |                                                           | 4. Automated grading system for objective questions.                         |
|     |                         |                                                           | 5. Real-time monitoring of quiz progress and participant performance.        |
|     |                         |                                                           | 6. Access to detailed reports and analytics for quizzes.                     |
|     |                         |                                                           | 7. Ability to provide instant feedback to quiz takers.                       |
|     |                         |                                                           | 8. User-friendly interface for quiz creation and management.                 |
| 2   |  Users      | A. Quiz Access and Interaction                            | 1. Easy access to available quizzes through a dashboard.                     |
|     |                         |                                                           | 2. Ability to take quizzes within a set timeframe.                           |
|     |                         |                                                           | 3. Receive immediate feedback after quiz submission.                         |
|     |                         |                                                           | 4. Access to quiz history and performance statistics.                        |
|     |                         |                                                           | 5. Mobile accessibility to take quizzes on different devices.                |
|     |                         |                                                           | 6. Secure login and user data protection.                                    |
        2. Use case

## Use case
        
![usecase1 (1)](https://github.com/user-attachments/assets/5b7d9314-4e40-40ae-888a-7077e36022c9)


## F. Database Architecture
### Data Dictionary

#### 1. User Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| User_id         | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each user       |
| Name            | VARCHAR(50)     | NOT NULL                    | User's name                           |
| Email           | VARCHAR(100)    | UNIQUE, NOT NULL            | Unique email address                  |
| Password        | VARCHAR(255)    | NOT NULL                    | Hashed password                       |
| Role            | ENUM('teacher', 'student') | NOT NULL         | Role of the user                      |
| created_at     | DATETIME         | NOT NULL, Default: CURRENT_TIMESTAMP                    | Date and time when the user was created.       |
| update_at     | DATETIME        | NULL, On Update: CURRENT_TIMESTAMP                        |  Date and time when the user last updated.       |


#### 2. Quiz Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| quiz_id         | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each quiz       |
| Title           | VARCHAR(100)    | NOT NULL                    | Title of the quiz                     |
| Description     | TEXT            | NULL                        | Overview of the quiz                  |
| quiz_code     | VARCHAR(20)           | NOT NULL                        | The code of the quiz                 |
| teacher_id      | INT             | Foreign key to User(user_id)| References the teacher who created the quiz    |
| Duration        | INT             | NOT NULL                    | Time allotted to complete the quiz (in minutes) |
| created_at      | DATETIME        | NOT NULL, Default: CURRENT_TIMESTAMP  | Timestamp of quiz created            |
| updated_at       |  DATETIME         | NULL, On Update: CURRENT_TIMESTAMP  | Timestamp of quiz updated  |

#### 3. Question Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| question_id     | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each question    |
| Quiz Id         | INT             | FOREIGN KEY (Quiz.Id)       | ID of the quiz the question belongs to |
| Question Text   | TEXT            | NOT NULL                    | Text of the question                  |
| Question Type   | ENUM('multiple-choice', 'true/false', 'short answer', 'essay') | NOT NULL | Type of the question |
| created_at      | DATETIME        |  NOT NULL, Default: CURRENT_TIMESTAMP| Timestamp of question was created  |
| updated_at      | DATETIME        |NULL, On Update: CURRENT_TIMESTAMP  |   Timestamp of question was updated   |


#### 4. Option (For multiple-choice questions)

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| option_id       | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each option in MCQ  |
| question_id         | INT             | FOREIGN KEY (question_id )       | References the question to which the option belongs.        |
| option_text        |VARCHAR(255)           | NOT NULL      | The text of the option.        |
| is_correct    | BOOLEAN      | NOT NULL, Default: 0                   | Indicates if the option is the correct answer. |


#### 5. Answer Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| answer_id           | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each submitted answer.      |
| question_id    | INT             | Foreign Key (FK) to Question(question_id)   | References the question this answer belongs to.     |
| student_id        | INT             | Foreign Key (FK) to User(user_id)     | References the student who submitted the answer.         |
| answer_text     | TEXT            |NULL                    | The student's submitted answer (for short answer questions).             |
| submitted_at      | DATETIME         | NOT NULL, Default: CURRENT_TIMESTAMP                    | Date and time when the answer was submitted. |


#### 6. Result Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| result_id    | INT             | Primary Key (PK), Auto Increment | Unique identifier for each quiz result.   |
| quiz_id       | INT             | Foreign Key (FK) to Quiz(quiz_id)       | References the quiz for which the result is recorded.|
| student_id   | INT            | Foreign Key (FK) to User(user_id)                 | References the student who took the quiz.                 |
| score   | DECIMAL(5,2) | NOT NULL | The score achieved by the student in the quiz. |
| submitted_at     | DATETIME        |  NOT NULL, Default: CURRENT_TIMESTAMP| Date and time when the quiz was submitted. |

### ERD
![image](https://github.com/user-attachments/assets/109079a9-cd61-4ff6-ab53-915d3fd806c8)


https://lucid.app/lucidchart/3e889906-07a0-4379-8582-ca841fd4d1a1/edit?viewport_loc=-1875%2C-1117%2C4013%2C1864%2C0_0&invitationId=inv_6f4efdd6-431a-4dd4-8b29-d3c807d0b104

 
