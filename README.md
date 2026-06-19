# 🌍 Volunteer Connect

## Modern Volunteer & NGO Management Platform

Volunteer Connect is a full-stack Volunteer Management System designed to streamline volunteer engagement, event coordination, attendance tracking, application management, and reporting.

Built using **Spring Boot 3**, **Spring Security**, **JWT Authentication**, **MySQL**, **JPA/Hibernate**, **Thymeleaf**, **HTML**, **CSS**, and **JavaScript**, the platform provides a secure and scalable solution for organizations managing volunteer-driven initiatives.

---

## 🚀 Features

### 👥 Volunteer Management
- Volunteer Registration
- Volunteer Profile Management
- Volunteer Search & Filtering
- Volunteer Participation Tracking
- Volunteer Information Updates

### 📅 Event Management
- Create Events
- Update Events
- Delete Events
- Manage Event Capacity
- Event Scheduling
- Event Registration Tracking

### 📝 Application Management
- Apply for Events
- Application Approval/Rejection
- Application Status Tracking
- Volunteer Event Assignments

### ✅ Attendance Management
- Attendance Marking
- Attendance Updates
- Attendance Reports
- Participation Analytics

### 📊 Dashboard Analytics
- Total Volunteers
- Active Events
- Pending Applications
- Attendance Statistics
- Volunteer Engagement Metrics

### 📈 Excel Report Generation
Generate downloadable Excel reports for:
- Volunteers
- Events
- Attendance
- Applications

Powered by Apache POI.

### 🔒 Security Features
- JWT Authentication
- Role-Based Access Control (RBAC)
- BCrypt Password Encryption
- Spring Security Authorization
- Secure REST APIs

---

# 🛠️ Technology Stack

## Backend
- Java 17
- Spring Boot 3
- Spring Security
- Spring Data JPA
- Hibernate
- JWT Authentication
- MySQL
- Lombok
- MapStruct
- Apache POI

## Frontend
- HTML5
- CSS3
- JavaScript (Vanilla JS)
- Thymeleaf

## Documentation
- Swagger OpenAPI

---

# 📂 Project Structure

```text
src
│
├── main
│   ├── java
│   │
│   └── com.volunteer.management
│       ├── config
│       ├── controller
│       ├── dto
│       ├── entity
│       ├── enums
│       ├── mapper
│       ├── repository
│       ├── security
│       ├── service
│       ├── util
│       └── exception
│
├── resources
│   ├── templates
│   │   ├── index.html
│   │   ├── login.html
│   │   ├── register.html
│   │   └── dashboard.html
│   │
│   ├── static
│   │   ├── css
│   │   ├── js
│   │   ├── images
│   │   └── assets
│   │
│   └── application.properties
│
└── build.gradle
```

---

# 🌐 Application URLs

### Landing Page
```text
http://localhost:8080/
```

### Login Page
```text
http://localhost:8080/login
```

### Register Page
```text
http://localhost:8080/register
```

### Dashboard
```text
http://localhost:8080/dashboard
```

### Swagger UI
```text
http://localhost:8080/swagger-ui/index.html
```

### OpenAPI Documentation
```text
http://localhost:8080/v3/api-docs
```

### Health Check
```text
http://localhost:8080/actuator/health
```

---

# 🔑 Authentication Flow

```text
User Registration
        ↓
Password Encryption (BCrypt)
        ↓
Stored in Database
        ↓
User Account Created
```

```text
User Login
        ↓
Authentication
        ↓
JWT Token Generation
        ↓
Token Returned
        ↓
Authorized Requests
```

---

# 👨‍💼 User Roles

## ADMIN

Capabilities:
- Manage Volunteers
- Manage Events
- Manage Applications
- Manage Attendance
- Generate Reports
- Access Dashboard Analytics
- Full Administrative Access

## VOLUNTEER

Capabilities:
- Register Account
- Login
- View Events
- Apply for Events
- Track Participation
- Manage Personal Profile

---

# 📊 Core Entities

## User

```text
id
fullName
email
password
role
enabled
```

## Volunteer

```text
id
phone
address
skills
availability
user_id
```

## Event

```text
id
title
description
location
eventDate
capacity
```

## Application

```text
id
volunteer_id
event_id
status
```

## Attendance

```text
id
volunteer_id
event_id
present
```

---

# 🔐 Security Architecture

```text
Client Request
      ↓
JWT Authentication Filter
      ↓
Spring Security
      ↓
Controllers
      ↓
Services
      ↓
Repositories
      ↓
Database
```

---

# ⚙️ Installation & Setup

## Clone Repository

```bash
git clone https://github.com/your-username/volunteer-connect.git
```

## Navigate to Project

```bash
cd volunteer-connect
```

## Configure Database

Update `application.properties`

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/volunteer_connect
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

## Run Application

Using Gradle:

```bash
./gradlew bootRun
```

or

```bash
gradlew bootRun
```

---

# 📈 Future Enhancements

- Email Notifications
- Event Reminder System
- Certificate Generation
- QR Code Attendance
- Volunteer Ranking System
- AI Volunteer Matching
- Real-Time Notifications
- Cloud Deployment
- Mobile App Integration
- Advanced Analytics Dashboard

---

# 🎯 Key Highlights

✔ Spring Boot 3 Architecture

✔ JWT Authentication & Authorization

✔ Role-Based Access Control (RBAC)

✔ RESTful API Design

✔ MySQL Database Integration

✔ Dashboard Analytics

✔ Excel Report Generation

✔ Swagger API Documentation

✔ Modern Responsive Frontend

✔ Production-Ready Security Configuration

---

## 👩‍💻 Developer

**Khushi Sen**

Engineering Student | Java Backend Developer | Spring Boot Enthusiast

---

⭐ If you found this project useful, consider giving it a star and contributing to future enhancements.
