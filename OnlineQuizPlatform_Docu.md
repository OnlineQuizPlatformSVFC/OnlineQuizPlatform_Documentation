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

 •Project Planning
  
      - To develop a project schedule and timeline
      - To Identify and Manage Risks 
      - To Define a Communication Plan

  •Project Monitoring and Control
  
       - Monitor Project Performance and Progress 
       - Control Issues and Changes
       - Monitor Budget and Resources 

  •Project Execution
  
       - Team Management and Coordination
       - Risk Mitigation and Response
       - Reporting and Stakeholder Communication

  •Project Closure
  
       - Finalize Deliverables and Documentation
       - Review and Evaluate the Project

Platform Development:

  •Frontend Development
  
       - Design and Development of User Interfaces 
       - Management of User Accounts and Verification
       - Editor and Creation Interface for Quizzes 
       - Features for Collaboration and Sharing of Quizzes

  • Backend Development
  
        - Security and Management of User Data
        - Quiz Data Archiving and Access
        - Quiz Content Management System 
        - Tracking and optimizing performance

  • Testing and Quality Assurance
  
        - Individual Component Unit Testing 
        - Acceptance Testing for Users (UAT) 
        - Testing for Load and Performance

  • Deployment and Maintenance
  
        - Configuring and Setup Infrastructure 
        - Release management and platform deployment
        - Bug Repair and Problem Solving 
        - Updates for the system and new features

Content Management:
 
  •Content Creation Tools
  
       - Interface for creating and editing questions
       - Quiz Content Management System
       - Ability to upload images and videos

  •Content Moderation
  
        - Procedure for Content Approval and Review
        - Identification and Avoidance of Spam
        - Systems for User Reporting and Feedback

  • Content Distribution and Sharing
  
        - Features for Quiz Sharing (Links, Social Media) 
        - Features for Collaboration When Creating Quizzes
        - Search and Content Discovery Features

Security and Privacy:
 
  • User Authentication and Authorization
  
        - Secure User Registration and Login 
        - Access Control Based on Roles for Various Users
        - Security and Management of Passwords

 •Data Encryption and Storage
 
        - Secure Data Encryption and Storage
        - Disaster Recovery and Data Backup

 •Security Testing and Vulnerability Management
 
        - Regular Security Audits and Penetration Testing
        - Patching and Vulnerability Management

Marketing and Launch:
 
 •Marketing Strategy and Plan
 
         - Identification and Segmentation of the Target Audience
         - Advertising Campaigns and Channels 
         - Social media Interaction and Content Marketing

 •Platform Launch and Promotion
 
          - Beta Testing and Gathering Input 
          - Public Introduction and Declaration 
          - User Acquisition and Growth Strategies

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
 
