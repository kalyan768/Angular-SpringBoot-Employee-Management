# Employee Management System

A full-stack **Employee Management System** built using **Angular** for the frontend and **Spring Boot** for the backend. The application provides a simple interface to create, view, update, and delete employee records.

## 🚀 Tech Stack

### Frontend

* Angular
* TypeScript
* HTML5
* CSS3
* Bootstrap

### Backend

* Java
* Spring Boot
* Spring Data JPA
* Hibernate
* REST API

### Database

* MySQL

### Tools

* Git & GitHub
* Visual Studio Code
* IntelliJ IDEA / Eclipse
* Postman

---

## ✨ Features

* Add new employees
* View all employees
* View employee details
* Update employee information
* Delete employees
* REST API integration between Angular and Spring Boot
* MySQL database integration
* Responsive and user-friendly interface

---

## 📂 Project Structure

```text
Angular-SpringBoot-Employee-Management/
│
├── angular-frontend/
│   ├── src/
│   ├── angular.json
│   ├── package.json
│   └── ...
│
├── springbootbackend/
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       └── resources/
│   ├── pom.xml
│   └── ...
│
├── .gitignore
└── README.md
```

---

## 🔄 Application Architecture

```text
┌──────────────────────┐
│      Angular UI      │
│      Frontend        │
└──────────┬───────────┘
           │
           │ HTTP / REST API
           ▼
┌──────────────────────┐
│    Spring Boot       │
│      Backend         │
└──────────┬───────────┘
           │
           │ JPA / Hibernate
           ▼
┌──────────────────────┐
│        MySQL         │
│       Database       │
└──────────────────────┘
```

---

# ⚙️ Getting Started

## Prerequisites

Make sure the following are installed:

* Java 17 or later
* Node.js
* Angular CLI
* MySQL
* Git

---

## 🛠️ Backend Setup

Navigate to the backend directory:

```bash
cd springbootbackend
```

Configure your MySQL database in:

```text
src/main/resources/application.properties
```

Example configuration:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/employee_management
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

Create the database in MySQL:

```sql
CREATE DATABASE employee_management;
```

Start the Spring Boot application:

```bash
mvn spring-boot:run
```

The backend will run on:

```text
http://localhost:8080
```

---

## 💻 Frontend Setup

Open another terminal and navigate to the Angular application:

```bash
cd angular-frontend
```

Install the required dependencies:

```bash
npm install
```

Start the Angular development server:

```bash
ng serve
```

Open your browser and visit:

```text
http://localhost:4200
```

---

# 🔗 API

The Angular frontend communicates with the Spring Boot backend through REST APIs.

Example base URL:

```text
http://localhost:8080/api/v1/employees
```

| Method | Endpoint                 | Description           |
| ------ | ------------------------ | --------------------- |
| GET    | `/api/v1/employees`      | Get all employees     |
| GET    | `/api/v1/employees/{id}` | Get employee by ID    |
| POST   | `/api/v1/employees`      | Create a new employee |
| PUT    | `/api/v1/employees/{id}` | Update an employee    |
| DELETE | `/api/v1/employees/{id}` | Delete an employee    |

---

# 🗄️ Employee Data

Each employee record contains information such as:

* Employee ID
* First Name
* Last Name
* Email

The data is stored in a MySQL database and accessed through Spring Data JPA.

---

# 📸 Screenshots

Add screenshots of your application here.

Recommended screenshots:

```text
screenshots/
├── employee-list.png
├── add-employee.png
├── update-employee.png
└── employee-details.png
```

---

# 🔮 Future Enhancements

* Employee search and filtering
* Pagination
* Form validation
* User authentication and authorization
* Role-based access control
* Improved responsive design
* Deployment to a cloud platform

---

# 👨‍💻 Author

**Mandadhi Kalyan**

GitHub: [@kalyan768](https://github.com/kalyan768)

---

## 📄 License

This project is created for learning and educational purposes.
