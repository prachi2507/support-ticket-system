🎫 Support Ticket System (Spring Boot)

A backend Support Ticket Management System built using Spring Boot, JPA, and MySQL (MariaDB).
This project demonstrates clean REST API design, database integration, enums usage, and CRUD operations — suitable for real-world enterprise applications.

🚀 Features

Create support tickets
View all tickets
View ticket by ID
Ticket status management using enums
Ticket priority handling
RESTful APIs tested via Postman
MySQL / MariaDB database integration using JPA & Hibernate

Tech Stack

Backend: Java, Spring Boot
Database: MySQL / MariaDB
ORM: Spring Data JPA (Hibernate)
Build Tool: Maven
API Testing: Postman
Server: Embedded Tomcat
Version Control: Git & GitHub

📁 Project Structure
support-ticket-system
│
├── controller
│   └── TicketController.java
│
├── entity
│   ├── Ticket.java
│   ├── TicketStatus.java
│   └── TicketPriority.java
│
├── repository
│   └── TicketRepository.java
│
├── SupportTicketSystemApplication.java
└── application.properties

🧾 Ticket Entity Fields
| Field       | Type                             |
| ----------- | -------------------------------- |
| id          | Long                             |
| title       | String                           |
| description | String                           |
| status      | Enum (OPEN, IN_PROGRESS, CLOSED) |
| priority    | Enum (LOW, MEDIUM, HIGH)         |
| createdAt   | LocalDateTime                    |

🔗 API Endpoints
Create Ticket

POST /api/tickets
{
  "title": "Login issue",
  "description": "Unable to login with valid credentials",
  "status": "OPEN",
  "priority": "HIGH"
}

Get All Tickets
GET /api/tickets

Get Ticket by ID
GET /api/tickets/{id}

Health Check
GET /test
Response:
App is running fine 🚀

🧪 Testing
All APIs were tested using Postman and validated against the MySQL database using phpMyAdmin.

🎯 Learning Outcomes
REST API design using Spring Boot
JPA entity relationships & enums
Handling validation & database constraints
Debugging Hibernate & MySQL errors
GitHub version control & project structuring

👩‍💻 Author
Prachi Bane
Java & Backend Developer
GitHub: https://github.com/prachi2507
