# AI-Powered Adaptive Learning and Personalized Course Recommendation System

## Team Details

| Team Member | ID Number |
|---|---|
| G. Sirisha | 2420030091 |
| D. Venkatesh | 2420030134 |
| A. Srinivas | 2420030136 |
| Y. Yamini | 2420030264 |

**Supervisor:** Rajkumar Patil

---

## Abstract

The **AI-Powered Adaptive Learning and Personalized Course Recommendation System** is a web-based application designed to provide personalized learning experiences based on students' interests, skills, academic performance, and learning progress.

Traditional online learning platforms generally provide the same courses and learning paths to all students without considering their individual learning requirements. Students have different levels of knowledge, learning speeds, interests, strengths, and weaknesses. Therefore, a common learning path may not be suitable for every student.

This project aims to overcome this limitation by developing an adaptive learning platform that analyzes student performance and recommends suitable courses based on individual requirements. The system allows students to register, create profiles, select interests, explore courses, complete quizzes and assessments, and track their learning progress.

The system analyzes quiz scores, completed courses, selected interests, skill levels, and topic-wise performance. Based on these factors, it identifies strong and weak areas and recommends suitable courses. As the student's performance changes, the system adapts the recommended course difficulty and learning path.

The application is developed using **React.js** for the frontend, **Spring Boot** for the backend, and **MySQL** for database management. An AI-based recommendation component is used to support personalized course recommendations. DevOps practices such as Git, GitHub, automated testing, CI/CD, Docker, and cloud deployment are integrated to support continuous development and delivery.

The main objective of the project is to make learning more **personalized, adaptive, and effective** by continuously analyzing student performance and recommending appropriate learning content.

---

## Problem Statement

Traditional learning platforms often provide generalized courses and recommendations to students without considering their individual learning requirements.

Students may differ in:

- Knowledge level
- Learning speed
- Interests
- Skills
- Academic performance
- Strengths and weaknesses
- Learning goals

As a result, students may receive courses that are too easy, too difficult, or unrelated to their current requirements.

Therefore, there is a need for an **adaptive learning platform** that can analyze student performance and continuously modify course recommendations according to individual learning needs.

---

## Proposed Solution

The proposed system provides a personalized learning environment that adapts according to each student's performance and preferences.

The system collects and analyzes:

- Student profile
- Learning interests
- Existing skills
- Quiz scores
- Assessment results
- Completed courses
- Topic-wise performance
- Learning progress

The recommendation engine uses this information to identify appropriate courses and create a personalized learning path.

### Example

| Subject | Score | Performance |
|---|---:|---|
| Python | 85% | Strong |
| Java | 72% | Good |
| DBMS | 42% | Weak |
| Networking | 65% | Moderate |

Based on this performance, the system may recommend:

```text
DBMS Fundamentals
        |
        v
SQL Basics
        |
        v
Database Normalization
        |
        v
Advanced DBMS
```

When the student's DBMS performance improves, the system can recommend more advanced courses.

---

## Technologies Used

| Category | Technology |
|---|---|
| Frontend | React.js |
| Backend | Spring Boot |
| Programming Language | Java |
| Database | MySQL |
| AI | AI / Recommendation Engine |
| API | REST API |
| Version Control | Git & GitHub |
| CI/CD | GitHub Actions |
| Testing | JUnit / Spring Boot Test |
| Containerization | Docker |
| Cloud | AWS |

---

## Project Objectives

- To develop a user-friendly adaptive learning platform.
- To provide personalized course recommendations.
- To analyze student performance and learning progress.
- To identify student strengths and weaknesses.
- To consider student interests and skill levels.
- To dynamically adapt course recommendations based on performance.
- To provide personalized learning paths.
- To track student learning progress.
- To manage student and course information efficiently.
- To demonstrate Adaptive Software Engineering principles.
- To integrate DevOps practices for continuous development and deployment.

---

## Key Features

| Feature | Description |
|---|---|
| Student Registration | Allows students to create an account |
| Student Login | Allows students to securely access the system |
| Student Profile | Stores student skills, interests, and learning information |
| Course Search | Allows students to search available courses |
| Course Details | Displays course information and difficulty |
| Quiz and Assessment | Evaluates student knowledge |
| Performance Tracking | Tracks quiz and course performance |
| Topic Analysis | Identifies strong and weak topics |
| Personalized Recommendation | Recommends suitable courses |
| AI-Based Recommendation | Uses AI/recommendation logic for personalization |
| Adaptive Difficulty | Adjusts course recommendations according to performance |
| Personalized Learning Path | Creates a personalized sequence of courses |
| Progress Tracking | Tracks completed and ongoing courses |
| Student Dashboard | Displays performance and recommendations |
| Database Management | Stores student, course, quiz, and recommendation data |
| Git-Based Development | Supports collaborative development |
| CI/CD Integration | Automates build and testing |
| Docker Deployment | Supports containerized deployment |

---

## Adaptive Learning Process

The system continuously adapts course recommendations according to the student's performance and learning progress.

### Adaptive Learning Flow

```text
                    STUDENT
                       |
                       v
             Student Profile
                       |
                       v
          Interests and Skill Level
                       |
                       v
              Quiz / Assessment
                       |
                       v
           Performance Analysis
                       |
                       v
        Identify Strengths & Weaknesses
                       |
                       v
           Recommendation Engine
                       |
                       v
        Personalized Course
             Recommendation
                       |
                       v
               Student Learns
                       |
                       v
             Course / Quiz
              Completion
                       |
                       v
           New Performance Data
                       |
                       v
          Update Student Profile
                       |
                       v
        Adapt Recommendations
                       |
                       v
          Recommend Next Course
```

---

## Adaptive Recommendation Logic

The initial version of the system can use performance-based rules to determine the appropriate course difficulty.

| Score | Learning Level | Recommendation |
|---|---|---|
| Below 40% | Beginner | Beginner-level course |
| 40% - 70% | Intermediate | Intermediate-level course |
| Above 70% | Advanced | Advanced-level course |

### Example

```text
Student Score = 35%
        |
        v
Beginner Level
        |
        v
Beginner Course
        |
        v
Student Completes Course
        |
        v
New Assessment
        |
        v
Student Score = 75%
        |
        v
Advanced Level
        |
        v
Advanced Course
```

This allows the platform to adapt its recommendations according to the student's latest performance.

---

## System Architecture

The system follows a layered architecture consisting of the Frontend Layer, Backend Layer, AI/Recommendation Layer, Database Layer, and DevOps Layer.

```text
┌─────────────────────────────────────────────────────────────┐
│                         USER LAYER                          │
│                                                             │
│                    Student / Administrator                  │
└─────────────────────────────┬───────────────────────────────┘
                              |
                              v
┌─────────────────────────────────────────────────────────────┐
│                    PRESENTATION LAYER                       │
│                                                             │
│                       React.js                              │
│                                                             │
│  Login | Profile | Courses | Quiz | Dashboard | Results     │
└─────────────────────────────┬───────────────────────────────┘
                              |
                         REST APIs
                              |
                              v
┌─────────────────────────────────────────────────────────────┐
│                    APPLICATION LAYER                        │
│                                                             │
│                     Spring Boot                             │
│                                                             │
│ Authentication | Student | Course | Quiz | Performance      │
│ Recommendation | Learning Path | Progress Management        │
└───────────────┬──────────────────────────┬──────────────────┘
                |                          |
                v                          v
┌───────────────────────────┐   ┌─────────────────────────────┐
│     AI / ADAPTIVE LAYER   │   │       DATABASE LAYER        │
│                           │   │                             │
│ Performance Analysis      │   │           MySQL             │
│ Recommendation Engine     │   │                             │
│ Learning-Level Analysis   │   │ Students                    │
│ Personalized Learning     │   │ Courses                     │
│                           │   │ Quizzes                     │
└───────────────┬───────────┘   │ Results                     │
                |               │ Preferences                 │
                |               │ Recommendations             │
                |               │ Learning Progress            │
                |               └─────────────────────────────┘
                |
                v
┌─────────────────────────────────────────────────────────────┐
│                       DEVOPS LAYER                          │
│                                                             │
│ Git → GitHub → CI/CD → Testing → Docker → AWS              │
│                                                             │
│              Deployment and Monitoring                      │
└─────────────────────────────────────────────────────────────┘
```

---

## System Components

### 1. Frontend

The frontend is developed using **React.js** and provides an interactive interface for students.

#### Student Interface

- Registration
- Login
- Student Profile
- Course Browsing
- Course Details
- Quiz
- Assessment Results
- Course Recommendations
- Learning Progress
- Dashboard

#### Administrator Interface

- Manage Students
- Add Courses
- Update Courses
- Delete Courses
- Manage Quizzes
- View Student Performance

---

### 2. Backend

The backend is developed using **Spring Boot**.

It handles:

- Authentication
- Student Management
- Course Management
- Quiz Management
- Performance Calculation
- Recommendation Requests
- Learning Progress
- REST API Communication
- Database Operations

---

### 3. AI / Recommendation Layer

The AI/recommendation layer analyzes student information and generates personalized recommendations.

It considers:

- Student interests
- Student skills
- Quiz performance
- Topic-wise scores
- Completed courses
- Current learning level
- Course difficulty

The recommendation engine then ranks suitable courses for the student.

---

### 4. Database Layer

MySQL is used to store and manage system data.

The database contains information about:

- Students
- Courses
- Student Preferences
- Skills
- Quizzes
- Questions
- Quiz Results
- Recommendations
- Learning Progress

---

## Database Design

The major entities of the system are:

```text
                    STUDENT
                       |
          ┌────────────┼────────────┐
          |            |            |
          v            v            v
     PREFERENCE    PERFORMANCE    PROGRESS
                       |
                       v
                      QUIZ
                       |
                       v
                     RESULT
                       |
                       v
                RECOMMENDATION
                       |
                       v
                     COURSE
```

### Main Database Tables

| Table | Purpose |
|---|---|
| Student | Stores student information |
| Course | Stores available courses |
| Preference | Stores student interests |
| Skill | Stores student skills |
| Quiz | Stores quiz information |
| Question | Stores quiz questions |
| Result | Stores quiz results |
| Recommendation | Stores recommended courses |
| Learning_Progress | Tracks student progress |

---

## Project Structure

```text
AI-Powered-Adaptive-Learning/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Login.jsx
│   │   │   ├── Register.jsx
│   │   │   ├── CourseCard.jsx
│   │   │   ├── Quiz.jsx
│   │   │   └── Recommendation.jsx
│   │   │
│   │   ├── pages/
│   │   │   ├── Home.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Courses.jsx
│   │   │   ├── Profile.jsx
│   │   │   └── Results.jsx
│   │   │
│   │   ├── services/
│   │   │   └── api.js
│   │   │
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── README.md
│
├── backend/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   └── resources/
│   │   │       └── application.properties
│   │   └── test/
│   │
│   ├── pom.xml
│   └── README.md
│
├── ai-service/
│   ├── app.py
│   ├── recommendation.py
│   ├── performance_analysis.py
│   ├── requirements.txt
│   └── README.md
│
├── database/
│   └── schema.sql
│
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── docs/
│   ├── requirements/
│   ├── architecture/
│   ├── database/
│   └── screenshots/
│
└── README.md
```

---

## API Architecture

The React frontend communicates with the Spring Boot backend through REST APIs.

| HTTP Method | Endpoint | Purpose |
|---|---|---|
| POST | `/api/auth/register` | Register a student |
| POST | `/api/auth/login` | Student login |
| GET | `/api/students/{id}` | Get student profile |
| PUT | `/api/students/{id}` | Update student profile |
| GET | `/api/courses` | Get all courses |
| GET | `/api/courses/{id}` | Get course details |
| POST | `/api/courses` | Add a course |
| PUT | `/api/courses/{id}` | Update a course |
| DELETE | `/api/courses/{id}` | Delete a course |
| GET | `/api/quizzes/{id}` | Get quiz |
| POST | `/api/results` | Submit quiz result |
| GET | `/api/results/{studentId}` | Get student results |
| GET | `/api/recommendations/{studentId}` | Get recommendations |
| GET | `/api/progress/{studentId}` | Get learning progress |

---

## AI Recommendation Workflow

```text
                Student Data
                     |
                     v
          ┌─────────────────────┐
          │ Performance Analysis│
          └──────────┬──────────┘
                     |
                     v
          ┌─────────────────────┐
          │ Identify Weak Areas │
          └──────────┬──────────┘
                     |
                     v
          ┌─────────────────────┐
          │ Analyze Interests   │
          └──────────┬──────────┘
                     |
                     v
          ┌─────────────────────┐
          │ Match Suitable      │
          │ Courses             │
          └──────────┬──────────┘
                     |
                     v
          ┌─────────────────────┐
          │ Rank Courses        │
          └──────────┬──────────┘
                     |
                     v
          ┌─────────────────────┐
          │ Personalized Course │
          │ Recommendations     │
          └─────────────────────┘
```

---

## DevOps Integration

The project follows DevOps practices to support continuous development, testing, integration, and deployment.

### DevOps Workflow

```text
                     Developer
                         |
                         v
                  GitHub Repository
                         |
                         v
                   Feature Branch
                         |
                         v
                    Pull Request
                         |
                         v
                    Code Review
                         |
                         v
                Automated Testing
                         |
                         v
                    CI Pipeline
                         |
                         v
                       Build
                         |
                         v
                  Docker Image
                         |
                         v
                    Deployment
                         |
                         v
                       AWS
                         |
                         v
                    Monitoring
                         |
                         v
                Continuous Improvement
```

### DevOps Technologies

| Technology | Purpose |
|---|---|
| Git | Version control |
| GitHub | Source code management |
| GitHub Actions | CI/CD automation |
| JUnit | Backend testing |
| Docker | Containerization |
| AWS | Cloud deployment |
| Monitoring Tools | Application monitoring |

---

## Setup and Execution Instructions

### Prerequisites

Make sure the following software is installed:

| Software | Purpose |
|---|---|
| Node.js | Frontend development |
| npm | Frontend package management |
| Java JDK 21 | Backend development |
| Maven | Backend build management |
| MySQL | Database |
| Git | Version control |
| Docker | Containerization |
| Visual Studio Code / IntelliJ IDEA | Development environment |

---

### 1. Clone the Repository

```bash
git clone <repository-url>
cd AI-Powered-Adaptive-Learning
```

---

### 2. Frontend Setup

Navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the React application:

```bash
npm run dev
```

If the project uses Create React App:

```bash
npm start
```

---

### 3. Database Setup

Open MySQL and create the database:

```sql
CREATE DATABASE adaptive_learning_db;
```

Configure the database connection in:

```text
backend/src/main/resources/application.properties
```

Example configuration:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/adaptive_learning_db
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

server.port=8080
```

Replace `your_password` with your MySQL password.

---

### 4. Backend Setup

Open a new terminal and navigate to the backend:

```bash
cd backend
```

Run the Spring Boot application:

```bash
mvn spring-boot:run
```

The backend will run on:

```text
http://localhost:8080
```

---

### 5. AI Service Setup

If a separate AI service is implemented, navigate to:

```bash
cd ai-service
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the service:

```bash
python app.py
```

---

### 6. Run the Complete Application

The complete system consists of:

```text
React Frontend
       |
       v
Spring Boot Backend
       |
       +------------------+
       |                  |
       v                  v
MySQL Database      AI Recommendation
                         Service
```

Start the frontend, backend, database, and AI service if applicable.

---

## Docker Setup

Build the Docker image:

```bash
docker build -t adaptive-learning-platform .
```

Run the Docker container:

```bash
docker run -p 8080:8080 adaptive-learning-platform
```

If Docker Compose is used:

```bash
docker compose up --build
```

---

## Testing Strategy

The project uses multiple levels of testing to ensure system reliability.

| Testing Type | Purpose |
|---|---|
| Unit Testing | Tests individual methods and components |
| Integration Testing | Tests communication between modules |
| API Testing | Tests REST API endpoints |
| Database Testing | Verifies database operations |
| UI Testing | Tests frontend functionality |
| System Testing | Tests the complete application |
| User Acceptance Testing | Validates system requirements |

---

## Expected Outcomes

The proposed system is expected to:

- Provide personalized course recommendations.
- Identify student strengths and weaknesses.
- Adapt course difficulty according to performance.
- Provide personalized learning paths.
- Track student learning progress.
- Improve student engagement.
- Improve learning efficiency.
- Reduce irrelevant course recommendations.
- Provide an adaptive learning environment.
- Support continuous software development through DevOps.

---

## Future Enhancements

Future versions of the system can include:

- AI chatbot for student doubts.
- Automatic quiz generation.
- Voice-based learning assistance.
- Mobile application.
- Advanced recommendation algorithms.
- Predictive student performance analysis.
- Gamification.
- Achievement and reward systems.
- Knowledge graph-based recommendations.
- Real-time learning analytics.
- Integration with external learning platforms.
- Advanced AI-based personalization.

---

## Current Phase Status

### Phase 1 – Project Planning and Requirement Analysis

**Status: In Progress**

### Completed

- [x] Team formation
- [x] Project topic selection
- [x] Problem identification
- [x] Project objectives
- [x] Abstract preparation
- [x] Technology selection
- [x] Initial project planning

### In Progress

- [ ] Requirement analysis
- [ ] Functional requirements
- [ ] Non-functional requirements
- [ ] System architecture design
- [ ] Database design
- [ ] UI/UX design
- [ ] GitHub repository setup

### Upcoming

- [ ] React frontend development
- [ ] Spring Boot backend development
- [ ] MySQL database integration
- [ ] Authentication
- [ ] Course management
- [ ] Quiz and assessment module
- [ ] Student performance analysis
- [ ] AI recommendation module
- [ ] Adaptive learning module
- [ ] Frontend-backend integration
- [ ] Automated testing
- [ ] CI/CD pipeline
- [ ] Docker integration
- [ ] Cloud deployment
- [ ] Final testing
- [ ] Project documentation

---

## Team Responsibilities

| Team Member | ID Number | Responsibility |
|---|---|---|
| G. Sirisha | 2420030091 | Project Coordination, Backend and DevOps |
| D. Venkatesh | 2420030134 | Frontend and UI/UX |
| A. Srinivas | 2420030136 | AI and Recommendation Module |
| Y. Yamini | 2420030264 | Database, Testing and Documentation |

---

## Project Summary

| Project Information | Details |
|---|---|
| Project Title | AI-Powered Adaptive Learning and Personalized Course Recommendation System |
| Domain | Artificial Intelligence, Adaptive Software Engineering and DevOps |
| Frontend | React.js |
| Backend | Spring Boot |
| Programming Language | Java |
| Database | MySQL |
| AI | AI / Recommendation Engine |
| API | REST API |
| Version Control | Git & GitHub |
| CI/CD | GitHub Actions |
| Containerization | Docker |
| Cloud | AWS |
| Team Size | 4 Members |
| Supervisor | Rajkumar Patil |

---

## Core Project Concept

The project combines **Adaptive Software Engineering, Artificial Intelligence, Personalized Learning, and DevOps**.

### Adaptive Learning Cycle

```text
Analyze
   |
   v
Recommend
   |
   v
Learn
   |
   v
Evaluate
   |
   v
Adapt
   |
   v
Recommend Again
```

### DevOps Cycle

```text
Code
   |
   v
Build
   |
   v
Test
   |
   v
Deploy
   |
   v
Monitor
   |
   v
Improve
   |
   └──────────────> Code Again
```

Together, these two cycles create a **continuously improving AI-powered adaptive learning platform** that responds to changing student requirements while supporting continuous software development, testing, and deployment.
