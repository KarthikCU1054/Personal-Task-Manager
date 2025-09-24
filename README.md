# Task Tracking Application

A Task Management System built with Spring Boot (backend) and a provided React frontend.
The app allows users to create task lists, add tasks with priorities and due dates, update their progress, and stay organized.

⸻

# Features
•	Task Lists: Create, update, delete task lists.
•	Tasks: Add, update, delete, and mark tasks as complete.
•	Progress Tracking: View completion percentage of each task list.
•	Priorities & Deadlines: Assign High/Medium/Low priority and due dates.
•	REST API: Backend built with Spring Boot + Spring Data JPA.
•	Database: PostgreSQL (running in Docker).
•	Frontend: React app (provided).
•	Error Handling: Centralized exception handling with consistent JSON responses.

⸻

# Tech Stack
•	Backend: Java 21, Spring Boot 3, Spring Data JPA
•	Database: PostgreSQL (Dockerized), H2 (for tests)
•	Build Tool: Maven
•	Frontend: React
•	Containerization: Docker & Docker Compose

⸻

# Project Structure

task-tracker/
├── backend/                # Spring Boot backend (your code)
│   ├── src/main/java/...   # Controllers, Services, Entities, DTOs, Mappers
│   ├── src/main/resources/ # application.properties
│   └── pom.xml             # Maven build file
├── frontend/               # Provided React frontend
│   ├── src/...
│   ├── package.json
│   └── vite.config.js
└── docker-compose.yml      # PostgreSQL container config

---

# REST API Endpoints

## Task Lists
•	GET    /task-lists → List all task lists
•	POST   /task-lists → Create new task list
•	GET    /task-lists/{id} → Get task list by ID
•	PUT    /task-lists/{id} → Update task list
•	DELETE /task-lists/{id} → Delete task list

## Tasks
•	GET    /task-lists/{taskListId}/tasks → List tasks in a list
•	POST   /task-lists/{taskListId}/tasks → Create new task
•	GET    /task-lists/{taskListId}/tasks/{taskId} → Get task by ID
•	PUT    /task-lists/{taskListId}/tasks/{taskId} → Update task
•	DELETE /task-lists/{taskListId}/tasks/{taskId} → Delete task

⸻

📸 Screenshots (Optional)

Add screenshots of the UI (task lists, tasks, progress bar).

⸻
