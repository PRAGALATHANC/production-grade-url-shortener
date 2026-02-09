# Production-Grade URL Shortener

A production-grade URL Shortener service built with Java, Spring Boot, MySQL, Redis, JWT Authentication, and Docker — designed with scalable architecture and performance optimization in mind.

---

## 🚀 Overview

This project implements a high-performance URL shortening backend service similar to bit.ly, with features including:

✔ URL creation with expiration support  
✔ Redirect to original URL  
✔ JWT-based authenticated APIs  
✔ Redis caching for fast lookup  
✔ Click analytics tracking  
✔ Rate limiting to prevent abuse  
✔ Containerized with Docker  
✔ Clean layered architecture for maintainability

---

## 🧱 Tech Stack

| Layer | Technology |
|-------|------------|
| Language | Java |
| Backend Framework | Spring Boot |
| Database | MySQL |
| Cache | Redis |
| Auth | JWT Authentication |
| Containerization | Docker & Docker Compose |
| DevOps | CI/CD Ready |

---

## 🗂 Project Structure

src/main/java/
├── config/ # App & Security configuration
├── controller/ # REST controllers
├── dto/ # Request & response models
├── exception/ # Custom exception handlers
├── model/ # JPA entities
├── repository/ # Data access layer
├── security/ # JWT & filter logic
├── service/ # Business logic services
└── util/ # Utilities (e.g., code generator)

---

## 🚧 Features

### 🔐 Authentication
- User signup
- Login with JWT token
- Secured endpoints with role validation

### 🔗 URL Shortening
- POST long URL → returns short URL
- GET short URL → redirects to original
- Expiry time support

### ⚡ Performance
- Redis caching for frequent lookups
- DB indexing for optimized queries

### 📊 Analytics
- Track number of clicks
- Store click metadata

### 🚫 Rate Limiting
- Prevent abuse with request thresholds

---

## 📦 Docker Setup (Recommended)

Ensure Docker & Docker-Compose are installed.

```sh
docker compose up -d
