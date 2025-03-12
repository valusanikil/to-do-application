# Todo Application with Spring Boot

This project is a simple **Todo Application** built using **Spring Boot**. The application allows users to manage their daily tasks, add new tasks, view existing tasks, and delete tasks. It provides a basic user authentication mechanism and stores todo items for each user session.

## Project Overview
This Todo application allows users to:
- Log in with a username and password.
- View a list of tasks (todos).
- Add a new task.
- Delete a task.

The app uses a simple **login service** for authentication and allows users to manage tasks through a **TodoService**. The **Spring MVC** framework handles HTTP requests, while **Spring’s Model-View-Controller (MVC) pattern** is used for rendering views and managing user input.

## Technologies Used
- **Spring Boot**: Framework for building Java-based applications.
- **Spring MVC**: To handle HTTP requests and serve views.
- **Java 8+**: Programming language used for backend logic.
- **Thymeleaf**: Template engine used to render HTML pages.
- **Model-View-Controller**: Design pattern used for separating the application's logic.
- **Maven**: Dependency management and build tool.

## Features
- **User Login**: A simple login mechanism for authentication. The username is "Nikil" and the password is "123456" (this can be customized as needed).
- **Add Todo**: Users can add new tasks with a description.
- **View Todos**: A list of todos associated with the logged-in user.
- **Delete Todo**: Users can delete tasks that are no longer needed.

## Setup and Installation
To run the Todo application locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/todo-app.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd todo-app
   ```

3. **Build and run the project** using Maven:
   ```bash
   mvn spring-boot:run
   ```

4. **Access the application**:
   Open your browser and visit `http://localhost:8080/login` to access the login page.

## Project Structure
The project is organized as follows:

```
todo-app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── in28minutes/
│   │   │           └── springboot/
│   │   │               └── web/
│   │   │                   ├── controller/
│   │   │                   │   ├── LoginController.java
│   │   │                   │   └── TodoController.java
│   │   │                   ├── model/
│   │   │                   │   └── Todo.java
│   │   │                   └── service/
│   │   │                       ├── LoginService.java
│   │   │                       └── TodoService.java
│   │   └── resources/
│   │       ├── static/
│   │       └── templates/
│   │           ├── login.html
│   │           ├── list-todos.html
│   │           ├── todo.html
│   │           └── welcome.html
├── pom.xml
└── README.md
```

### Key Classes:
- **LoginController.java**: Manages login functionality.
- **TodoController.java**: Handles todo-related operations such as listing, adding, and deleting todos.
- **Todo.java**: Represents the `Todo` entity.
- **LoginService.java**: Validates the login credentials.
- **TodoService.java**: Manages the list of todos, adds and deletes tasks.


## Screenshots
<img src="assets/Screenshot 2025-03-12 092121.png" alt="">
