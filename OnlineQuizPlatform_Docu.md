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
      
    •The online quiz platform may face limitations in customization for complex quiz formats and handling large user loads, which could impact performance. Security challenges such as preventing 
     cheating and data breaches could affect reliability. Limited offline functionality means users need a stable internet connection, restricting access in areas with poor connectivity. 
     

## D. Work breakdown Structure
The main actions involved in creating an online quiz platform are delineated in this Work Breakdown Structure (WBS). The project is divided into manageable parts by it's hierarchical structure.

![image](https://github.com/user-attachments/assets/11518cf3-96cd-4585-b922-61b2a4ba4dee)


## E. Functional Requirements

        1. User  Requirements
| No. | Users                   | System Features                                           | Requirement                                                                 |
|-----|-------------------------|-----------------------------------------------------------|------------------------------------------------------------------------------|
| 1   | Educators/Instructors    | A. Quiz Management                                        | 1. Ability to create and customize quizzes with different types of questions (multiple-choice, true/false, short answer, essay). |
|     |                         |                                                           | 2. Capability to schedule quizzes for specific dates and times.              |
|     |                         |                                                           | 3. Option to set time limits for each quiz.                                   |
|     |                         |                                                           | 4. Automated grading system for objective questions.                         |
|     |                         |                                                           | 5. Real-time monitoring of quiz progress and participant performance.        |
|     |                         |                                                           | 6. Access to detailed reports and analytics for quizzes.                     |
|     |                         |                                                           | 7. Ability to provide instant feedback to quiz takers.                       |
|     |                         |                                                           | 8. User-friendly interface for quiz creation and management.                 |
| 2   | Students/Participants    | A. Quiz Access and Interaction                            | 1. Easy access to available quizzes through a dashboard.                     |
|     |                         |                                                           | 2. Ability to take quizzes within a set timeframe.                           |
|     |                         |                                                           | 3. Receive immediate feedback after quiz submission.                         |
|     |                         |                                                           | 4. Access to quiz history and performance statistics.                        |
|     |                         |                                                           | 5. Mobile accessibility to take quizzes on different devices.                |
|     |                         |                                                           | 6. Secure login and user data protection.                                    |
| 3   | Administrators           | A. System Management                                      | 1. Manage user roles and permissions (e.g., educators, students).            |
|     |                         |                                                           | 2. Monitor system performance and user activity.                             |
|     |                         |                                                           | 3. Ensure data security and handle backup processes.                         |
|     |                         |                                                           | 4. Manage platform settings, including language and appearance customization. |
        2. Use case

## Use case
        
![usecase1 (1)](https://github.com/user-attachments/assets/5b7d9314-4e40-40ae-888a-7077e36022c9)


## F. Database Architecture
### Data Dictionary

#### 1. User Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| Id              | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each user       |
| First Name      | VARCHAR(50)     | NOT NULL                    | User's first name                     |
| Middle Name      | VARCHAR(50)     | NULL                        | Optional middle name                 |
| Last Name       | VARCHAR(50)     | NOT NULL                    | User's last name                      |
| Email           | VARCHAR(100)    | UNIQUE, NOT NULL            | Unique email address                  |
| Password        | VARCHAR(255)    | NOT NULL                    | Hashed password                       |
| Role            | ENUM('instructor', 'administrator', 'student') | NOT NULL | Role of the user                      |
| Registered      | DATETIME        | NOT NULL                    | Timestamp of user registration        |
| Last Login      | DATETIME        | NULL                        | Timestamp of last user login          |
| Profile Picture | VARCHAR(255)    | NULL                        | URL of the user's profile picture     |

#### 2. Quiz Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| Id              | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each quiz        |
| Title           | VARCHAR(100)    | NOT NULL                    | Title of the quiz                     |
| Description     | TEXT            | NULL                        | Overview of the quiz                  |
| Category        | VARCHAR(50)     | NULL                        | Topic or category of the quiz         |
| Difficulty      | ENUM('easy', 'medium', 'hard') | NULL      | Difficulty level of the quiz          |
| Duration        | INT             | NOT NULL                    | Time allotted to complete the quiz (in minutes) |
| Created By      | INT             | FOREIGN KEY (User.Id)       | User ID of the quiz creator            |
| Created         | DATETIME        | NOT NULL                    | Timestamp of quiz creation            |
| Published       | BOOLEAN         | DEFAULT FALSE               | Flag indicating if the quiz is published |

#### 3. Question Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| Id              | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each question    |
| Quiz Id         | INT             | FOREIGN KEY (Quiz.Id)       | ID of the quiz the question belongs to |
| Question Text   | TEXT            | NOT NULL                    | Text of the question                  |
| Question Type   | ENUM('multiple-choice', 'true/false', 'short answer', 'essay') | NOT NULL | Type of the question                  |
| Options         | JSON            | NULL                        | Options for multiple-choice questions (if applicable) |
| Correct Answer  | TEXT            | NOT NULL                    | Correct answer for the question       |

#### 4. Answer Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| Id              | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each answer      |
| Question Id     | INT             | FOREIGN KEY (Question.Id)   | ID of the question being answered      |
| User Id         | INT             | FOREIGN KEY (User.Id)       | ID of the user who answered            |
| Answer Text     | TEXT            | NOT NULL                    | Text of the user's answer             |
| Is Correct      | BOOLEAN         | NOT NULL                    | Flag indicating if the answer is correct |

#### 5. Attempt Table

| Column Name     | Data Type      | Constraints                | Description                           |
|-----------------|-----------------|-----------------------------|---------------------------------------|
| Id              | INT             | PRIMARY KEY, AUTO_INCREMENT | Unique identifier for each attempt     |
| Quiz Id         | INT             | FOREIGN KEY (Quiz.Id)       | ID of the quiz being attempted         |
| User Id         | INT             | FOREIGN KEY (User.Id)       | ID of the user taking the quiz         |
| Start Time      | DATETIME        | NOT NULL                    | Timestamp of when the attempt started  |
| End Time        | DATETIME        | NOT NULL                    | Timestamp of when the attempt ended    |
| Score           | DECIMAL(5, 2)   | NULL                        | Final score of the attempt            |
| Duration        | INT             | NOT NULL                    | Time taken to complete the quiz (in minutes) |


### ERD

![image](https://github.com/user-attachments/assets/5a982074-2607-4839-b148-f921b8bdf8f8)

 
