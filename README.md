ORDER MANAGEMENT SYSTEM

📌 Overview
This project is a web-based backend application that manages product orders using a modern and scalable architecture.
It demonstrates how to build a RESTful API with secure authentication, event-driven communication, and containerized deployment using industry-standard technologies.

🎯 Objectives
Build a secure and scalable REST API
Implement event-driven architecture using Kafka
Manage relational data using SQL Server
Track system activities with logging and analytics
Containerize services using Docker

🚀 Features
🔐 Authentication & Authorization (JWT-based)
👤 User Management
📦 Product Management
🛒 Order Management (Create & track orders)
⚡ Event-Driven Architecture (Kafka integration)
📜 Event Logging
📊 Analytics Dashboard (basic)
🧾 Audit Logging
🐳 Dockerized Environment

⚙️ Tech Stack
Technology
Purpose
.NET Core Web API
Backend API development
JWT
Authentication & authorization
SQL Server
Relational database
Kafka
Event streaming & messaging
Docker
Containerization
Git
Version control


🏗️ Architecture
The system follows a layered architecture combined with event-driven design:
Client sends request to API
API processes request and stores data in SQL Server
API publishes event to Kafka
Kafka consumer processes the event
Events are stored for logging and analytics

🧱 Database Structure (Simplified)
Users → Store user accounts
Products → Store product data
Orders → Store order information
OrderItems → Store order details
EventLogs → Store Kafka events
AuditLogs → Track user activity

▶️ Getting Started
🔧 Prerequisites
.NET 8 SDK
Docker & Docker Compose
SQL Server
Kafka

▶️ Run with Docker
docker-compose up --build

▶️ Run API Locally
dotnet restore
dotnet build
dotnet run

🔑 API Authentication
Register a new user
Login to get JWT token
Use token in headers:
Authorization: Bearer {your_token}

📡 Example Event Flow
User creates an order
API saves order to database
API publishes order_created event to Kafka
Consumer processes the event
Event is stored in EventLogs

📊 Sample Use Cases
Track order lifecycle
Monitor system activity via logs
Analyze order trends
Demonstrate event-driven architecture

🐳 Docker Services
API Service
SQL Server
Kafka Broker

📌 Future Improvements
Payment integration
Email notification system
Advanced analytics dashboard
Role-based permission enhancement

👨‍💻 Author
Developed as a portfolio project to demonstrate backend engineering skills using .NET and modern system design.


