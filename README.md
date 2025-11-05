# Todo App - Spring Boot Project

A full-stack **Todo List** application built using:

* **Spring Boot** for backend logic and RESTful services
* **Thymeleaf** for dynamic server-side rendering
* **Bootstrap** for responsive UI design
* **MySQL** for persistent data storage

---

## Overview

This project is a simple yet complete CRUD-based web application for managing daily tasks.
Users can create, update, mark as complete/incomplete, and delete tasks.
It demonstrates the core features of a typical Spring Boot MVC application with database integration and a responsive front-end.

---

## Features

* Add, edit, and delete tasks
* Mark tasks as **complete** or **incomplete**
* Responsive and user-friendly interface using **Bootstrap**
* Data persistence using **MySQL**
* MVC pattern using **Spring Boot + Thymeleaf**
* Validation and exception handling

---

## Tech Stack

| Layer      | Technology                                |
| ---------- | ----------------------------------------- |
| Backend    | Spring Boot (Spring MVC, Spring Data JPA) |
| Frontend   | Thymeleaf + Bootstrap                     |
| Database   | MySQL                                     |
| Build Tool | Maven                                     |
| Language   | Java 17+                                  |

---

## Project Structure

```
src/
 ├─ main/
 │   ├─ java/com/example/todo
 │   │   ├─ controller/        # Web controllers
 │   │   ├─ model/             # Entity classes
 │   │   ├─ repository/        # JPA repositories
 │   │   └─ service/           # Business logic
 │   └─ resources/
 │       ├─ templates/         # Thymeleaf HTML pages
 │       ├─ static/            # CSS, JS, and Bootstrap files
 │       └─ application.properties
 └─ test/
```

---

## Database Configuration

Update your database credentials in `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
```

---

## Run Instructions

1. Clone the repository:

   ```bash
   git clone <repo-url>
   cd todo-app
   ```

2. Configure the database in `application.properties`

3. Run the application using Maven:

   ```bash
   mvn spring-boot:run
   ```

4. Open your browser and navigate to:

   ```
   http://localhost:8080
   ```

---

## Example Pages

* **Home Page** – Displays all tasks
* **Add Task Page** – Form to add new todo item
* **Edit Task Page** – Update existing task
* **Delete Functionality** – Deletes task permanently

---

## Future Enhancements

* Add user authentication
* Implement REST API endpoints
* Add due dates and categories
* Integrate with frontend framework (React / Angular)

---

## License

This project is licensed under the MIT License.
You are free to use, modify, and distribute it with attribution.

---
