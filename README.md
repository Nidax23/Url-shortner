URL Shortener Platform | Spring Boot, JWT, REST APIs, Docker

A **production-ready full-stack URL Shortener application** built using **Java, Spring Boot, Spring Security, JWT authentication, RESTful APIs, MySQL, Docker, and cloud deployment**.

The project demonstrates **backend system design**, **secure authentication**, **user-specific data handling**, **analytics tracking**, and **end-to-end deployment**, following **industry-standard practices**.

##  Tech Stack 

**Backend**

* Java
* Spring Boot
* Spring Security
* JWT (JSON Web Token)
* RESTful APIs
* Hibernate / JPA
* MySQL

**Frontend**

* React
* Tailwind CSS
* Context API

**DevOps & Tools**

* Docker
* Git & GitHub
* Maven
* Cloud Database
* Linux Server

### Features

**Authentication & Authorization**

* User registration and login
* JWT token generation and validation
* Role-based access control
* Custom Spring Security configuration
* Stateless authentication

**URL Management**

* URL shortening logic
* Secure redirect functionality
* Public and private URLs
* Path-based routing

**Analytics & Dashboard**

* Click tracking per URL
* User-level analytics
* URL-specific performance insights
* Dashboard data APIs

**Deployment**

* Dockerized backend application
* Cloud-hosted database
* Domain routing and server deployment
* End-to-end tested system

### System Architecture & Workflow

**End-to-End Request Flow**

```
User
 │
 │  (Login / Signup)
 ▼
Frontend (React + Tailwind)
 │
 │  JWT Token
 ▼
Spring Boot Backend
 │
 ├── Authentication Controller
 │   └── JWT Generation
 │
 ├── Security Layer
 │   ├── JWT Filter
 │   ├── UserDetailsService
 │   └── Spring Security Config
 │
 ├── Business Logic Layer
 │   ├── URL Shortening Service
 │   ├── Redirect Service
 │   └── Analytics Service
 │
 ▼
Database (MySQL / Cloud)
 ├── Users
 ├── URLs
 └── Click Logs
```

### Backend Setup

```bash
git clone https://github.com/Nidax23/Url-shortner.git
cd url-shortener-project
```

Configure `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/url_db
spring.datasource.username=root
spring.datasource.password=your_password

jwt.secret=your_secret_key
jwt.expiration=172800000
```

Run the application:

```bash
mvn spring-boot:run
```

---

## Application Usage

1. Register a new user
2. Authenticate and receive JWT token
3. Create shortened URLs
4. Access short URLs for redirection
5. View analytics on dashboard

---

## Security Implementation Details

* JWT-based stateless authentication
* Custom authentication filter
* Secure API endpoints
* Role-based authorization
* Spring Security best practices
---

##  Future Enhancements

* Redis caching for faster redirects
* Rate limiting to prevent abuse
* QR code generation
* Admin analytics dashboard
* Custom short URL aliases


