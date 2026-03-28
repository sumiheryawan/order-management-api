# 🚀 Order Management System

```md
![.NET](https://img.shields.io/badge/.NET-8-blue)
![Docker](https://img.shields.io/badge/Docker-Enabled-blue)
![Kafka](https://img.shields.io/badge/Kafka-Event--Driven-orange)


## 📌 Overview
Order Management System is a web-based backend application designed to manage product orders using a **modern and scalable architecture**.

This project demonstrates how to build a **RESTful API** with:
- Secure authentication (JWT)
- Event-driven communication (Kafka)
- Containerized deployment (Docker)

---

## 🎯 Objectives
- Build a secure and scalable REST API
- Implement event-driven architecture using Kafka
- Manage relational data using SQL Server
- Track system activities with logging & analytics
- Containerize services using Docker

---

## 🚀 Features
- 🔐 Authentication & Authorization (JWT-based)
- 👤 User Management
- 📦 Product Management
- 🛒 Order Management (Create & Track Orders)
- ⚡ Event-Driven Architecture (Kafka Integration)
- 📜 Event Logging
- 📊 Basic Analytics Dashboard
- 🧾 Audit Logging
- 🐳 Dockerized Environment

---

## ⚙️ Tech Stack

| Technology          | Purpose                          |
|--------------------|----------------------------------|
| .NET Core Web API  | Backend API development          |
| JWT                | Authentication & Authorization   |
| SQL Server         | Relational Database              |
| Kafka              | Event Streaming & Messaging      |
| Docker             | Containerization                 |
| Git                | Version Control                  |

---

## 🏗️ Architecture

The system uses a **Layered Architecture** combined with **Event-Driven Design**:

1. Client sends request to API  
2. API processes request & stores data in SQL Server  
3. API publishes event to Kafka  
4. Kafka consumer processes the event  
5. Events are stored for logging & analytics  


---

## ▶️ Getting Started

### 🔧 Prerequisites
- .NET 8 SDK
- Docker & Docker Compose
- SQL Server
- Kafka

---

### 🐳 Run with Docker
```bash
docker-compose up --build