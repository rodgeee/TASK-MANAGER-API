# Task Manager API

This project is a simple Task Manager REST API developed using Symfony, API Platform, and Docker.  
It allows users to create tasks, update them, and mark tasks as completed through RESTful endpoints.

---

## Requirements
- Docker & Docker Compose
- Git

---

## Installation & Setup

### 1. Clone the repository
```bash
git clone <your-repository-url>
cd task-manager-api
2. Run the Docker containers
docker compose up -d --build
3. Enter the PHP container
docker compose exec php bash
4. Run database migrations
php bin/console make:migration
php bin/console doctrine:migrations:migrate
API Documentation
Once the containers are running, open your browser and go to:

http://localhost/api
The API Platform interface allows you to:

Create a task (POST)

View all tasks (GET)

Update a task (PUT)

Mark a task as completed (PATCH)

Database
Database name: task_manager_api

Managed using MySQL inside Docker

phpMyAdmin is available for database inspection

Docker Setup
The application runs using Docker containers:

PHP – Symfony application

MySQL – Database

phpMyAdmin – Database management tool

To check running containers:

docker compose ps
Author