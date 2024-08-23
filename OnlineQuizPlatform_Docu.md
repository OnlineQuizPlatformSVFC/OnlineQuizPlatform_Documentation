# HERONS LIBRARY: University of Makati Managing Library App Transaction

## INTRODUCTION

The library is a vital part of any university because it provides a space for students and teachers
to study, conduct research, and access various resources. There have been many library initiatives in
almost every part of the world. A library management system is software made specifically to control
every aspect of a library. It aids librarians in maintaining a database of newly released books as well as
books that members have borrowed and their due dates. This system fully automates each activity in your
library. Implementing a library management system software is the best approach to systematically
maintaining, arranging, and handling innumerable books. Records for libraries are kept up to date using a
library management system. It keeps track of the number of books in the library, how many are issued,
how many are returned or renewed, how many have late fines assessed, etc.

Library Manage system is software that books can be quickly located, issued, or reissued, and all
the data can be managed effectively and efficiently. A library management system's goal is to provide
information instantly and accurately about any type of book, saving a great deal of time and effort. Having
the User management module, recording logs or activities inside the library such as reading, researching,
skimming and SDI (Selection Dissemination Information), borrowing books, and other resources would
not be time-consuming as before. Also, the User Management Module will keep track of the user’s details.
Catalog Module, which provides the list of the materials and resources available. Circulation Management
Module that provides the QR code of the materials or book that the user is going to borrow. And OPAC
(Online Public Access Catalog) that enables users to access the application anywhere and anytime they
want to check and explore the available materials the library can provide.

## Project Features and Characteristics
The proposed project Umak Library Mobile App consists of the following features:
1. Catalog Module - recording and monitoring of resources - librarian
2. User management module - logs - user
3. Circulation management module - generate qr and scan qr by the students for borrowing of
resources using Qr code - librarian and student
4. OPAC - searching - student
5. Reports - number of borrowers librarian
   a. Daily, weekly, monthly and semestral reports

## Project Scope

UMak Library Management System is proposed to provide a function that helps the librarian and the
student be productive and efficient with their tasks inside the University's Library. These cover the data
of the student, library materials and resources, and records of activities inside the library. In order to
support and provide the library with accurate data, efficient organizing and tracking of lists of records,
and track the activities within the library. The system may be provided to the Head librarian, library
staff, and to the College students of Umak.

However, the system only allows the student users to access the list of available resources and
materials that they can borrow insider the library, they cannot bring home the books outside the library
because it does not allow the student to do so. Currently the system does not provide e-books that can
be downloaded since it will affect the library data privacy. Only students can use or borrow the materials
inside the library.



## Work breakdown Structure

![image](https://github.com/user-attachments/assets/9c490c78-6f5f-46a9-965d-c6aa8a0941a5)

## Functional Requirements

### User Requirements

| No. | Users      | System Features                                          | Requirement                                                                                                                                               |
|-----|------------|----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1   | Librarian  | A. User Management Module - Register Borrowers           | 1. The system must allow the Librarian to register the students on the mobile application by entering:                                                      |
|     |            |                                                          |    a. Umak Email address                                                                                                                                   |
|     |            |                                                          |    b. Name                                                                                                                                                 |
|     |            |                                                          |    c. Password                                                                                                                                             |
|     |            |                                                          |    d. Address                                                                                                                                              |
|     |            |                                                          |    e. Phone Number                                                                                                                                         |
|     |            |                                                          |    f. College                                                                                                                                              |
|     |            |                                                          |    g. Course                                                                                                                                               |
|     |            |                                                          |    h. Section                                                                                                                                              |
|     |            | B. User Management Module - Borrower Details             | 2. The system must allow the Librarian to view borrower details:                                                                                           |
|     |            |                                                          |    a. Borrower ID                                                                                                                                          |
|     |            |                                                          |    b. Record of Borrowed Books                                                                                                                             |
|     |            |                                                          |    c. Record of Activity Logs                                                                                                                              |
|     |            |                                                          |    d. Borrower Section                                                                                                                                     |
|     |            |                                                          |    e. Borrower Course                                                                                                                                      |
|     |            |                                                          |    f. Borrower College                                                                                                                                     |
|     |            | C. User Management Module - History of Borrowers         | 3. The system must allow the Librarian to view the history of the borrower’s account:                                                                      |
|     |            |                                                          |    a. Borrower Name                                                                                                                                        |
|     |            |                                                          |    b. Book Name                                                                                                                                            |
|     |            | D. Catalog Module - Register Book                        | 4. The system must allow the Librarian to write:                                                                                                           |
|     |            |                                                          |    a. Name                                                                                                                                                 |
|     |            |                                                          |    b. Author                                                                                                                                               |
|     |            |                                                          |    c. Publisher                                                                                                                                            |
|     |            |                                                          |    d. Published Date                                                                                                                                       |
|     |            |                                                          |    e. Description                                                                                                                                          |
|     |            |                                                          |    f. Location                                                                                                                                             |
|     |            |                                                          |    g. Genre                                                                                                                                                |
|     |            |                                                          |    h. Category                                                                                                                                             |
|     |            | E. Circulation Management Module                         | 5. The system must allow the Librarian to accept borrowers to borrow books by entering:                                                                    |
|     |            |                                                          |    a. Borrower name                                                                                                                                        |
|     |            |                                                          |    b. Borrower email                                                                                                                                       |
|     |            |                                                          |    c. Borrower College                                                                                                                                     |
|     |            |                                                          |    d. Borrower Course                                                                                                                                      |
|     |            |                                                          |    e. Borrower Section                                                                                                                                     |
|     |            |                                                          |    f. Book Title                                                                                                                                           |
|     |            | F. Report                                                | 6. The system must allow the Librarian to view the dashboard with the following reports:                                                                    |
|     |            |                                                          |    a. Daily Report                                                                                                                                         |
|     |            |                                                          |    b. Weekly Report                                                                                                                                        |
|     |            |                                                          |    c. Monthly Report                                                                                                                                       |
|     |            |                                                          |    d. Semestral Report                                                                                                                                     |
| 2   | Borrowers  | A. User Management Module - Login                        | 1. The system must allow the borrowers to log in to the mobile application by entering:                                                                    |
|     |            |                                                          |    a. Email address                                                                                                                                        |
|     |            |                                                          |    b. Password                                                                                                                                             |
|     |            | B. OPAC - View                                           | 2. The system must allow the borrowers to view books, including:                                                                                           |
|     |            |                                                          |    a. Name of the books                                                                                                                                    |
|     |            |                                                          |    b. Recommended books                                                                                                                                    |
|     |            |                                                          |    c. Category books                                                                                                                                       |
|     |            |                                                          |    d. Popular books                                                                                                                                        |
|     |            | C. OPAC - Search                                         | 3. The system must allow the borrowers to search for books by entering:                                                                                    |
|     |            |                                                          |    a. Book Name                                                                                                                                            |
|     |            |                                                          |    b. Author                                                                                                                                               |
|     |            | D. Circulation Management Module                         | 4. The system must allow the borrowers to borrow the books by generating:                                                                                  |
|     |            |                                                          |    a. QR Code                                                                                                                                              |

### use case
![image](https://github.com/user-attachments/assets/8229f510-9130-42a0-a054-2f689662dd7a)

## Database Architecture

### Data Dictionary
### Table 1: ACCOUNT_TYPE

| FIELD NAME | DESCRIPTION                          | DATA TYPE | LENGTH | SAMPLE        |
|------------|--------------------------------------|-----------|--------|---------------|
| USER_ID    | Unique Identification of User        | String    | 255    | FDSFDSF1233   |
| TYPE       | Identify if borrower or librarian    | String    | 55     | Borrower      |
| STATUS     | Identify online or Offline           | Boolean   |        | True          |
| CREATED    | Datetimestamp of user Created        | Date      |        | 11 2 2022 13:01 |

### Table 2: LIBRARIAN

| FIELD NAME        | DESCRIPTION                   | DATA TYPE | LENGTH | SAMPLE                |
|-------------------|-------------------------------|-----------|--------|-----------------------|
| LIBRARIAN_ID      | Librarian identification number| String    | 255    | ADEUWYE232            |
| NAME              | Librarian Name                | String    | 255    | Raiden Guillergan     |
| LIBRARIAN_EMAIL   | Librarian Email               | String    | 255    | guillergan@umak.edu.ph|
| DEPARTMENT        | Librarian Department          | String    | 255    | CCIS                  |

### Table 3: BORROWER

| FIELD NAME   | DESCRIPTION                            | DATA TYPE | LENGTH | SAMPLE                   |
|--------------|----------------------------------------|-----------|--------|--------------------------|
| BORROWER_ID  | Borrower identification number         | String    | 255    | ADHASDH384323            |
| USERNAME     | Borrower Username. It is shown in rating instead of Fullname | String | 255 | Thirdy454 |
| FIRSTNAME    | Borrower first name                    | String    | 255    | Jose                     |
| EMAIL        | Borrower Email                         | String    | 255    | Jgayares.a12034879@umak.edu.ph |
| LASTNAME     | Borrower last name                     | String    | 255    | Gayares                  |
| SECTION      | Borrower section                       | String    | 255    | III-ACDS                 |
| COURSE       | Borrower course                        | String    | 255    | CDS                      |
| COLLEGE      | Borrower college department            | String    | 255    | CCIS                     |
| ADDED_BY     | Librarian name who registered the borrower | String | 255 | Raiden Guillergan        |

### Table 4: BOOKS

| FIELD NAME  | DESCRIPTION                               | DATA TYPE | LENGTH | SAMPLE                                                           |
|-------------|-------------------------------------------|-----------|--------|------------------------------------------------------------------|
| BOOK_ID     | Book identification number                | String    | 255    | 2367284DGSHFG                                                    |
| CODE        | QR CODE OR BAR CODE to easily track the book | String  | 255    | 1232fdsfw3                                                       |
| TITLE       | Title of the book                         | String    | 255    | Noli Me tangere                                                  |
| AUTHOR      | Author of the book                        | String    | 255    | Jose Rizal                                                       |
| IMAGE       | Link of Image of the books                | String    | 255    | https://firebase.com/image.png                                   |
| PUBLISHER   | Publisher of the book                     | String    | 255    | Jonny Company                                                    |
| PUBLISHED DATE | Published date of the book            | Date      |        | July 8 1970                                                      |
| DESCRIPTION | Description of the book                   | String    | 255    | Noli me tangere is a novel by Filipino author and patriot Jose Rizal |
| CATEGORY    | Genre of the book to easily recommend to borrowers | String | 255 | Technology                                                       |
| LOCATION    | Category of the book (uses Dewey decimal) | String    | 255    | 0123                                                             |
| AVAILABLE   | Availability of the book, whether it has been borrowed by other borrowers or not | Boolean | | false |
| CREATED     | Datestamp When the books were created     | Date      |        | 11 22 2022, 10:02                                                |
| RATING_TOTAL| Total rating of the book                  | Int       | 55     | 513                                                              |
| RATING_AVERAGE| Rating average of the book             | Float     | 55     | 5                                                                |

### Table 5: BORROW

| FIELD NAME       | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|------------------|----------------------------------|-----------|--------|----------------|
| BOOKS_BORROWED_ID| Book borrowed identification number | STRING | 255    | DHSJKDHJSH     |
| BOOKS_ID         | Book identification number       | STRING    | 255    | DNSJDHJSHUTY   |
| BORROWER_ID      | Borrower identification number   | STRING    | 255    | FJSHFSGFGS     |
| LIBRARIAN_ID     | Librarian identification number  | STRING    | 255    | DHSJKDHJSUT    |
| BORROW_DATE      | Book borrowed date and time      | DATE      | 255    | 11 22 2022, 10:02 |
| RETURN_DATE      | Book return date and time        | DATE      | 255    | 11 22 2022, 12:02 |

### Table 6: LIBRARIAN_LOGS

| FIELD NAME       | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|------------------|----------------------------------|-----------|--------|----------------|
| LIBRARY_LOGS_ID  | Unique Identification of LOGS    | String    | 255    | FSFFWWRD       |
| ACTIVITIES       | Activities created by Librarian  | String    | 255    | Register Borrowers |
| LIBRARIAN_ID     | Getting the ID of users          | String    | 255    | DJSKADHSD2     |
| DATE_TIMESTAMP   | Generated date and time created  | Date      |        | 11 8 2022 19:01 |

### Table 7: BORROWER_LOGS

| FIELD NAME         | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|--------------------|----------------------------------|-----------|--------|----------------|
| BORROWERS_LOGS_ID  | Unique Identification of LOGS    | String    | 255    | FSFFWWRD       |
| ACTIVITIES         | Activities inside Library        | String    | 255    | SDI            |
| BORROWERS_ID       | Getting the ID of borrowers      | String    | 255    | HDUSYD23       |
| LIBRARIAN_ID       | Getting the ID of librarian      | String    | 255    | JDAHSDHD       |
| DATETIMESTAMP      | Date                             | Date      |        | 11 12 2022 13:01 |

### Table 8: NOTIFICATION

| FIELD NAME       | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|------------------|----------------------------------|-----------|--------|----------------|
| NOTIFICATION_ID  | Unique Identification of ID      | String    | 255    | DHASJKHDJSK    |
| TYPE             | Id of Book                       | String    | 255    | Borrow         |
| MESSAGE          | The message of Notification      | String    | 255    | You Borrow a book "Noli Me Tangere" |
| ID               | Type of Id                       | String    | 255    | GHDHFSGDD      |
| CREATED          | Notification Created             | Date      |        | 12 12 2022, 17:02 |

### Table 9: FAVORITES

| FIELD NAME          | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|---------------------|----------------------------------|-----------|--------|----------------|
| BOOKS_FAVORITES_ID  | Book Favorites identification number | String | 255    | HDJASDGS723    |
| BOOKS_ID            | Books identification number      | String    | 255    | DHSUDIGSD62    |
| BORROWER_ID         | Borrower identification number   | String    | 255    | JDISYDDCHJSDH  |

### Table 10: QRCODE_STORE

| FIELD NAME       | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|------------------|----------------------------------|-----------|--------|----------------|
| QRCODE_ID        | Unique Identification of LOGS    | String    | 255    | FSFFWWRD       |
| TYPE             | Type of QRCODE                   | String    | 255    |                |
| STATUS           | If available or expired the qrcode | Boolean |        | true           |
| ID               | The ID of the choosing type      | String    | 255    | SDSDFSFS2      |
| CREATED          | Datestamp of QR CODE CREATED     | Date      |        | 12 12 2022     |

### Table 11: RATING

| FIELD NAME       | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|------------------|----------------------------------|-----------|--------|----------------|
| RATING_ID        | Unique Identification of ID      | String    | 255    | DHASJKHDJSK    |
| BOOK_ID          | Id of Book                       | String    | 255    | DSDHISHDD      |
| BORROWER_ID      | User Id of Borrower              | String    | 255    | DJSJDHSDH      |
| RATE             | Rate of the borrower's in the book 1-5 | Int  | 1  | 5 |
| COMMENT          | Comment of the borrower's in the book | String | 255    | This book is awesome |
| CREATED          | Rate Created                     | Date      |        | 12 12 2022     |

### Table 12: LEADERBOARD

| FIELD NAME       | DESCRIPTION                      | DATA TYPE | LENGTH | SAMPLE         |
|------------------|----------------------------------|-----------|--------|----------------|
| LEADERBOARD_ID   | Leaderboard identification number | String   | 255    | DSDWRFJ2       |
| BOOKS_ID         | Books identification number      | String    | 255    | DSFSFW2FG      |
| BORROWER_ID      | Borrower identification number   | String    | 255    | MNBGGHJHGG     |
| POINTS           | Borrower Points                  | Int       | 55     | 5              |
| CATEGORY         | Point Category                   | String    | 255    | Borrow         |



## ERD

For Best View
https://www.figma.com/file/OXqoeVy3G1U1d3NSjdelYO/UMAK-LIBRARY-ERD?node-
id=0%3A1&t=rUvRxPi6Dcy35dHu


![image](https://github.com/user-attachments/assets/d4f53445-c2bd-4a6f-830f-5dd8e2177959)


## Non Functional Requirements

### Product Requirement (PLEASE SKIP THIS)

### Organizational Requirement (PLEASE SKIP THIS)


### External Requirements  (PLEASE SKIP THIS)


## System Testing and Evaluation   (PLEASE SKIP THIS)

### Functional Testing Procedure   (PLEASE SKIP THIS)

### Functional Testing Summary

### Evaluation Procedure

### Recommendation






### Wireframe (PLEASE SKIP THIS)



### High Fidelity (PLEASE SKIP THIS)



### System Screenshot (PLEASE SKIP THIS)
