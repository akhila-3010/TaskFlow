# TaskFlow – Scalable Task Management System

## Overview

TaskFlow is a full-stack task management application built as part of a Backend Developer Internship assignment. The project demonstrates secure authentication, role-based access control (RBAC), RESTful API design, database management, and frontend integration.

The application allows users to register, authenticate using JWT tokens, and manage tasks through a protected dashboard. Administrators have elevated privileges to manage all tasks and users.

---

## Features

### Authentication & Authorization

* User Registration
* User Login
* Password Hashing using bcrypt
* JWT Authentication
* Role-Based Access Control (User/Admin)

### Task Management

* Create Tasks
* View Tasks
* Update Tasks
* Delete Tasks
* Task Priority Management (High, Medium, Low)
* Filter Tasks by Status and Priority

### Frontend

* User Registration & Login Pages
* Protected Dashboard
* Task Management Interface
* Success and Error Notifications

### Security

* Password Encryption
* JWT Protected Routes
* Input Validation & Sanitization
* Error Handling Middleware

### API Features

* RESTful API Design
* API Versioning (/api/v1)
* Modular Architecture
* Swagger/Postman Documentation

---

## Tech Stack

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication
* bcrypt

### Frontend

* React.js
* Axios
* React Router

### Deployment

* Render

---

## Project Structure

backend/
├── config/
├── controllers/
├── middleware/
├── models/
├── routes/
├── services/
├── utils/
└── server.js

frontend/
├── src/
│ ├── pages/
│ ├── components/
│ ├── services/
│ └── App.js

---

## Installation

### Clone Repository

git clone https://github.com/akhila-3010/TaskFlow.git

### Backend Setup

cd backend
npm install
npm run dev

### Frontend Setup

cd frontend
npm install
npm run dev

---

## API Endpoints

### Authentication

POST /api/v1/auth/register

POST /api/v1/auth/login

### Tasks

GET /api/v1/tasks

POST /api/v1/tasks

PUT /api/v1/tasks/:id

DELETE /api/v1/tasks/:id

---

## Database Schema

### User

* name
* email
* password
* role

### Task

* title
* description
* priority
* status
* createdBy

---

## Scalability Notes

This application follows a modular architecture that separates routes, controllers, middleware, and database models for maintainability and scalability.

Future enhancements include:

* Redis Caching
* Docker Containerization
* Load Balancing
* Microservice-Based Architecture
* Centralized Logging and Monitoring
* CI/CD Pipeline Integration

---

## Deployment

Live Application:

https://task-manager-rfo2.onrender.com

---

## Author

Akhila Chinta

Backend Developer Internship Assignment Submission
