AI-Powered Adaptive Learning and Personalized Course Recommendation System

Team Details
## Team Details

| **Team Member** | **ID Number** |
| ---------------- | ------------- |
| G. Sirisha | 2420030091 |
| D. Venkatesh | 2420030134 |
| A. Srinivas | 2420030136 |
| Y. Yamini | 2420030264 |

**Supervisor:** Rajkumar Patil



Abstract

The AI-Powered Adaptive Learning and Personalized Course Recommendation System is a web-based application designed to provide personalized learning experiences based on students' interests, skills, academic performance, and learning progress. Traditional learning platforms generally provide the same courses and learning paths to all students without considering their individual learning requirements. This project aims to overcome this limitation by adapting course recommendations according to each student's performance, preferences, and learning needs.

The system allows students to register and log in, create their learning profiles, explore available courses, complete quizzes or assessments, and provide their interests and skill levels. Based on the student's performance and preferences, the platform identifies strong and weak areas and recommends suitable courses. The recommendation system can adapt the difficulty level of recommended courses as the student's performance changes.

The application is developed using React.js for the frontend, Spring Boot for the backend, and MySQL for database management. React.js provides an interactive and user-friendly interface, while Spring Boot handles the application logic and REST APIs. MySQL stores student details, course information, assessment results, preferences, and recommendation data. Artificial Intelligence can be integrated to analyze student performance and improve personalized recommendations.

The main objective of the project is to make learning more personalized, effective, and adaptive by continuously analyzing student performance and recommending suitable learning content based on individual requirements.

Technologies Used

Frontend: React.js
Backend: Spring Boot
Database: MySQL
AI: AI/Recommendation Engine
Version Control: Git and GitHub
DevOps: GitHub Actions, Docker, CI/CD

Project Objectives

To develop a user-friendly adaptive learning platform.
To provide personalized course recommendations.
To analyze student performance and learning progress.
To identify students' strengths and weaknesses.
To consider student interests, skills, and learning preferences.
To dynamically adapt course recommendations based on performance.
To provide personalized learning paths for students.
To store and manage student and course information efficiently.
To demonstrate the principles of Adaptive Software Engineering.
To integrate DevOps practices for continuous development and deployment.

Key Features

Student Registration and Login
Student Profile Management
Skill and Interest Selection
Course Search and Exploration
Course Details
Quiz and Assessment
Student Performance Tracking
Topic-Wise Performance Analysis
Personalized Course Recommendations
AI-Based Recommendation
Adaptive Course Difficulty
Personalized Learning Path
Strong and Weak Topic Identification
Learning Progress Tracking
Recommended Courses Dashboard
Database Management
Git-Based Version Control
CI/CD Integration
Docker-Based Deployment

Adaptive Learning Process

The system continuously adapts recommendations according to student performance.

Student Performance
        ↓
Performance Analysis
        ↓
Identify Strengths and Weaknesses
        ↓
Course Recommendation
        ↓
Student Completes Course / Quiz
        ↓
New Performance Data
        ↓
Update Student Profile
        ↓
Adapt Recommendations
        ↓
Recommend Next Course

For example:

Score < 40%
        ↓
Beginner-Level Course


Score 40% - 70%
        ↓
Intermediate-Level Course


Score > 70%
        ↓
Advanced-Level Course

This allows the platform to continuously adapt to the student's learning progress.

DevOps Integration

The project can use DevOps practices to support continuous development, testing, and deployment.

Developer
    ↓
GitHub Repository
    ↓
Feature Branch
    ↓
Pull Request
    ↓
Automated Testing
    ↓
CI Pipeline
    ↓
Build
    ↓
Docker
    ↓
Deployment
    ↓
Monitoring

The DevOps implementation helps the team maintain the project efficiently and deliver updates continuously.

Setup and Execution Instructions
Prerequisites

Make sure the following software is installed:

Node.js and npm
Java JDK
Maven
MySQL
Git
Docker
Visual Studio Code / IntelliJ IDEA
1. Clone the Repository
git clone <repository-url>
cd <project-folder>
2. Frontend Setup

Navigate to the React frontend directory:

cd frontend

Install the required dependencies:

npm install

Start the React application:

npm start

If the project uses Vite:

npm run dev
3. Database Setup

Open MySQL and create the project database:

CREATE DATABASE adaptive_learning_db;

Configure the database connection in the Spring Boot application.

File:

src/main/resources/application.properties

Example configuration:

spring.datasource.url=jdbc:mysql://localhost:3306/adaptive_learning_db
spring.datasource.username=root
spring.datasource.password=your_password


spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

Replace your_password with your MySQL password.

4. Backend Setup

Navigate to the Spring Boot backend directory:

cd backend

Run the Spring Boot application using Maven:

mvn spring-boot:run

The backend will start on the configured server port.

5. AI Recommendation Module

If the project contains a separate AI service, navigate to the AI service directory:

cd ai-service

Install the required Python dependencies:

pip install -r requirements.txt

Run the AI service:

python app.py

The AI service can communicate with the Spring Boot backend through REST APIs.

6. Run the Application

Start both the Spring Boot backend and React frontend.

If an AI service is included, start that service as well.

The React frontend communicates with the Spring Boot backend through REST APIs, while Spring Boot connects to the MySQL database.

The application can then be accessed through the frontend URL displayed in the terminal/browser.

Project Structure
AI-Powered-Adaptive-Learning/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       └── resources/
│   ├── pom.xml
│   └── ...
│
├── ai-service/
│   ├── app.py
│   ├── requirements.txt
│   └── ...
│
├── database/
│   └── schema.sql
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
└── README.md
Current Phase Status
Phase 1 – Project Planning and Requirement Analysis

Status: In Progress

Completed
Team formation
Project topic selection
Problem identification
Project objectives defined
Abstract prepared
Technology selection
Initial project planning
In Progress
Requirement analysis
Functional requirement identification
System architecture design
Database design
UI design
Project repository setup
Recommendation system planning
Upcoming
React frontend development
Spring Boot backend development
MySQL database integration
Student authentication
Course management module
Quiz and assessment module
Student performance analysis
Recommendation module development
Adaptive learning module
Frontend-backend integration
AI integration
Automated testing
CI/CD pipeline
Docker integration
Testing and debugging
Final deployment
Project documentation
Team

G. Sirisha — 2420030091

D. Venkatesh — 2420030134

A. Srinivas — 2420030136

Y. Yamini — 2420030264

Supervisor: Rajkumar Patil
