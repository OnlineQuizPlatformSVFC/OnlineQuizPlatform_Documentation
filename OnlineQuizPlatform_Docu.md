## A. Introduction
The online quiz platform aims to provide a simple digital solution for teachers to create, manage and distribute quizzes to students. The platform allows students to take online quizzes, receive instant feedback and track their progress. The goal is to enhance the learning experience by providing a flexible and interactive environment for teachers and students. The system will also simplify grading, reduce paper usage, and facilitate classification of quiz materials.

## B. Project Features and Characteristics

Project Features:

 User Management

         Registration and Login: Easy sign-up with email.

         User Profiles: Personalized dashboards with progress tracking.

         Role-Based Access: Differentiated access for students, teachers, and admins.


Quiz Creation and Management

        Custom Quiz Builder: Supports multiple question types and formats.

        Question Bank: Central repository for reusable questions.

        Randomization: Shuffle questions and answers to prevent cheating.

        Timed Quiz: Set time limits for quizzes or individual questions.
        

User Experience (UX)

     Responsive Design: Accessible on all devices (desktop, mobile).

     Intuitive Interface: User-friendly design for easy navigation.


Notifications
     
     Email and SMS Alerts: notifications for quiz deadlines and results.

     Customer Support: Access to email, or phone. 
     


Project Characteristics:

    User-Friendly: Focused on providing an accessible and intuitive user experience.

    Scalable: Designed to support a large number of users and quizzes.

    Secure: Prioritizes user data protection with robust security features.


## C. Project Scope

The Online Quiz Platform is an all-inclusive web application created to make it easier to create, administer, and take part in online quizzes. With a tools for making and administering quizzes, taking quizzes, getting feedback, and analyzing outcomes, this platform will serve both administrators and users to strong security measures, an intuitive user interface, and an adaptable question management system that supports a range of question kinds and difficulty levels will all be features of the platform.

The platform will also be made to be universally accessible, adaptable, and responsive to mobile devices. A fully working web application, thorough documentation, extensive testing, and training materials to guarantee successful implementation and usage are all part of the project deliverables.


   

## D. Work breakdown Structure
The main actions involved in creating an online quiz platform are delineated in this Work Breakdown Structure (WBS). The project is divided into manageable parts by its hierarchical structure.

flowchart TB
    subgraph Project_Management
        A[Project Planning]
        B[Project Monitoring and Control]
        C[Project Execution]
        D[Project Closure]
        
        A --> A1[Develop Project Schedule and Timeline]
        A --> A2[Identify and Manage Risks]
        A --> A3[Define Communication Plan]

        B --> B1[Monitor Project Performance and Progress]
        B --> B2[Control Issues and Changes]
        B --> B3[Monitor Budget and Resources]

        C --> C1[Team Management and Coordination]
        C --> C2[Risk Mitigation and Response]
        C --> C3[Reporting and Stakeholder Communication]

        D --> D1[Finalize Deliverables and Documentation]
        D --> D2[Review and Evaluate the Project]
    end
    
    subgraph Platform_Development
        E[Frontend Development]
        F[Backend Development]
        G[Testing and Quality Assurance]
        H[Deployment and Maintenance]

        E --> E1[Design and Development of User Interfaces]
        E --> E2[Management of User Accounts and Verification]
        E --> E3[Editor and Creation Interface for Quizzes]
        E --> E4[Features for Collaboration and Sharing of Quizzes]

        F --> F1[Security and Management of User Data]
        F --> F2[Quiz Data Archiving and Access]
        F --> F3[Quiz Content Management System]
        F --> F4[Tracking and Optimizing Performance]

        G --> G1[Individual Component Unit Testing]
        G --> G2[Acceptance Testing for Users (UAT)]
        G --> G3[Testing for Load and Performance]

        H --> H1[Configuring and Setup Infrastructure]
        H --> H2[Release Management and Platform Deployment]
        H --> H3[Bug Repair and Problem Solving]
        H --> H4[Updates for System and New Features]
    end
    
    subgraph Content_Management
        I[Content Creation Tools]
        J[Content Moderation]
        K[Content Distribution and Sharing]

        I --> I1[Interface for Creating and Editing Questions]
        I --> I2[Quiz Content Management System]
        I --> I3[Ability to Upload Images and Videos]

        J --> J1[Procedure for Content Approval and Review]
        J --> J2[Identification and Avoidance of Spam]
        J --> J3[Systems for User Reporting and Feedback]

        K --> K1[Features for Quiz Sharing (Links, Social Media)]
        K --> K2[Features for Collaboration When Creating Quizzes]
        K --> K3[Search and Content Discovery Features]
    end
    
    subgraph Security_and_Privacy
        L[User Authentication and Authorization]
        M[Data Encryption and Storage]
        N[Security Testing and Vulnerability Management]

        L --> L1[Secure User Registration and Login]
        L --> L2[Access Control Based on Roles for Various Users]
        L --> L3[Security and Management of Passwords]

        M --> M1[Secure Data Encryption and Storage]
        M --> M2[Disaster Recovery and Data Backup]

        N --> N1[Regular Security Audits and Penetration Testing]
        N --> N2[Patching and Vulnerability Management]
    end
    
    subgraph Marketing_and_Launch
        O[Marketing Strategy and Plan]
        P[Platform Launch and Promotion]

        O --> O1[Identification and Segmentation of Target Audience]
        O --> O2[Advertising Campaigns and Channels]
        O --> O3[Social Media Interaction and Content Marketing]

        P --> P1[Beta Testing and Gathering Input]
        P --> P2[Public Introduction and Declaration]
        P --> P3[User Acquisition and Growth Strategies]
    end



## E. Functional Requirements

        1. User  Requirements
        Educators/Instructors:
        * Ability to create and customize quizzes with different types of questions (multiple-choice, true/false, short answer, essay).
        * Capability to schedule quizzes for specific dates and times.
        * Option to set time limits for each quiz.
        * Automated grading system for objective questions.
        * Real-time monitoring of quiz progress and participant performance.
        * Access to detailed reports and analytics for quizzes.
        * Ability to provide instant feedback to quiz takers.
        * User-friendly interface for quiz creation and management.

        Students/Participants:
        * Easy access to available quizzes through a dashboard.
        * Ability to take quizzes within a set timeframe.
        * Receive immediate feedback after quiz submission.
        * Access to quiz history and performance statistics.
        * Mobile accessibility to take quizzes on different devices.
        * Secure login and user data protection.
        
        Administrators:
        * Manage user roles and permissions (e.g., educators, students).
        * Monitor system performance and user activity.
        * Ensure data security and handle backup processes.
        * Manage platform settings, including language and appearance customization.
        2. Use case

## F. Database Architecture

 1. User Table: Information about users is stored in this table, which includes:
 
 Id: A distinct identifier for every person
 
 First Name: The first name of the user
 
 Middle Name: The optional middle name of the user
 
 Last Name: The last name of the user
 
 Email: The user's distinct email address
 
 Password: An authenticating password that has been securely hashed
 
 Role: User role (e.g., instructor, administrator, student)
 
 Registered: A timestamp that represents the day of the user's registration
 
 Last Login: The user's most recent login time
 
 Profile Picture: The optional URL for the user's profile image
     
2.Quiz Table:
This table contains quiz-related information, such as:

 Id: A special number assigned to each quiz.
 
 Title: The quiz's title
 
 Description: An overview of the test
 
 Category: The quiz's topic or category
 
 Difficulty: The quiz's degree of difficulty (easy, medium, hard, etc.)
 
 Duration: The allotted time to finish the quiz.
 
 Created By: A foreign key that points to the User table and identifies who made the quiz
 
 Created: A timestamp that represents the day the quiz was created
 
 Published: A flag designating the quiz's public accessibility.
 
3. Question Table:





4. Answer Table:




5. Attempt Table:











Data Dictionary
 ERD
 
