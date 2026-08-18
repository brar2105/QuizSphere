QuizSphere 🎯

QuizSphere is a full-stack online quiz platform designed to provide an interactive and user-friendly way to conduct online quizzes. The application allows users to register, log in, access quizzes, answer multiple-choice questions, and manage quiz results.

The project follows a layered backend architecture where a React.js frontend communicates with a Java Spring Boot backend through REST APIs.


##  What Are We Building?

QuizSphere is designed as a complete quiz management system in which the **frontend, backend, and database work together** to provide a smooth quiz experience.

The frontend is responsible for the user interface and interactions, while the Spring Boot backend handles business logic, REST APIs, and database operations.

**H2 Database** is used as the relational database during development, with **Spring Data JPA and Hibernate** handling persistence and ORM.


##  What Has Been Implemented?

-User Management — User registration, user retrieval, and login functionality.
- Quiz Management — APIs for creating and managing quizzes.
- Question Management — Multiple-choice questions with four options and correct answers.
- Result Management — Stores quiz scores and total number of questions.
- REST APIs — Backend functionality exposed through RESTful endpoints.
- Database Integration — H2 database integrated using Spring Data JPA.
- ORM — Hibernate used for mapping Java objects to database tables.
- Responsive UI — React.js and CSS used to build the frontend interface.
- Frontend–Backend Communication — Fetch API used to communicate with backend APIs.



QuizSphere follows a **client-server architecture**:


                   


                  User
                      ↓
              React.js Frontend
                      ↓
                  Fetch API
                      ↓
            Spring Boot REST APIs
                      ↓
               Controller Layer
                      ↓
                Service Layer
                      ↓
              Repository Layer
                      ↓
          Spring Data JPA / Hibernate
                      ↓
                H2 Database
When a user performs an action on the frontend, such as logging in or interacting with a quiz, the React application sends a request to the appropriate Spring Boot REST API.
The Controller Layer receives the request and passes it to the Service Layer, where the application logic is handled. The Repository Layer communicates with the H2 database through Spring Data JPA and Hibernate.
The processed response is then returned to the React frontend and displayed to the user.
🛠️ Technologies Used
Frontend
React.js — Used to build the interactive user interface.
Vite — Used as the frontend development and build tool.
React Router — Used for client-side navigation.
HTML5 & CSS3 — Used for structuring, styling, and responsive design.
Fetch API — Used for frontend–backend API communication.
Backend
Java 17 — Primary programming language.
Spring Boot — Used to build the backend application and REST APIs.
Spring Data JPA — Used for database access and repository operations.
Hibernate — Used as the ORM framework.
Maven — Used for dependency management and project building.
Database
H2 Database — Lightweight relational database used during development and testing.

🗂️ Project Structure
QuizSphere/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── backend/
│   └── quizSphere/
│       ├── src/=
│       │   └── main/
│       │       ├── java/
│       │       │   └── com/komal/quizSphere/
│       │       │       ├── controller/
│       │       │       ├── service/
│       │       │       ├── repository/
│       │       │       └── entity/
│       │       │
│       │       └── resources/
│       │
│       └── pom.xml
│
└── README.md






🗄️ Database Design
QuizSphere currently uses four main entities:
Entity
Purpose
User
Stores user name, email, password, and role
Quiz
Stores quiz title and description
Question
Stores questions, options, and correct answers
Result
Stores quiz score and total questions

The relationships between these entities are managed using JPA annotations and Hibernate.

🏗️ Backend Architecture
The backend follows a clean layered structure:
Controller Layer
Handles HTTP requests and exposes REST endpoints for users, quizzes, questions, and results.
Service Layer
Contains application logic and acts as a bridge between controllers and repositories.
Repository Layer
Uses Spring Data JPA repositories to perform database operations.
Entity Layer
Contains JPA entity classes representing the application's database tables.
This separation makes the application easier to maintain, understand, test, and extend.

🔄 Application Flow
User Action
    ↓
React Component
    ↓
Fetch API Request
    ↓
Spring Boot REST Controller
    ↓
Service Layer
    ↓
JPA Repository
    ↓
H2 Database
    ↓
Response
    ↓
React UI

🎯 Project Objectives
Integrate a relational database using Spring Data JPA.The main objectives of QuizSphere are to:
Build a complete full-stack web application.
Implement RESTful APIs using Spring Boot.
Connect a React frontend with a Java backend.

Understand ORM using Hibernate.
Implement a layered backend architecture.
Practice real-world frontend–backend communication.
📚 Learning Outcomes
Working on QuizSphere provided practical experience with:
Full-stack web development
React.js and Vite
Spring Boot
REST API development
Spring Data JPA
Hibernate ORM
H2 relational database
Frontend–backend integration
Layered architecture
Maven project management
