# ToDoApp-SpringBoot

# TodoApp - A Simple Spring Boot Todo Application

## Overview
TodoApp is a simple task management application built using Spring Boot, Spring Data JPA, and Thymeleaf. It allows users to add, delete, and toggle the completion status of tasks.

## Features
- Add new tasks
- Mark tasks as completed or incomplete
- Delete tasks
- Persistent storage using MySQL
- Simple and responsive UI using Bootstrap and Thymeleaf

## Technologies Used
- **Spring Boot** - Backend framework
- **Spring Data JPA** - ORM for database interaction
- **Thymeleaf** - Server-side templating
- **Bootstrap** - Frontend styling
- **MySQL** - Relational database



## Setup Instructions
### Prerequisites
Ensure you have the following installed:
- Java 17 or later
- MySQL Server
- Maven

### Database Configuration
Update `src/main/resources/application.properties` with your MySQL credentials:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/todo-app
spring.datasource.username=your-username
spring.datasource.password=your-password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
```

### Running the Application
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/todoapp.git
   ```
2. Navigate to the project directory:
   ```sh
   cd todoapp
   ```
3. Build the project using Maven:
   ```sh
   mvn clean install
   ```
4. Run the application:
   ```sh
   mvn spring-boot:run
   ```
5. Open your browser and visit:
   ```
   http://localhost:8080
   ```

## API Endpoints
| Method | Endpoint         | Description                  |
|--------|-----------------|------------------------------|
| GET    | `/`             | Displays all tasks          |
| POST   | `/`             | Creates a new task          |
| GET    | `/{id}/delete`  | Deletes a task              |
| GET    | `/{id}/toggle`  | Toggles task completion     |


## Author
Samihan Jawalkar

