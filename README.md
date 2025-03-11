# Microservices Architecture with Spring Boot

This repository demonstrates a microservices architecture using **Spring Boot** and **Spring Cloud**, including essential components such as **Eureka Service Registry, Config Server, API Gateway, Spring Security, Zipkin Server**, and **Admin Server**.

## 📌 Features
- **Service Registry (Eureka Server)** - Enables service discovery and registration.
- **Config Server** - Centralized configuration management for all microservices.
- **API Gateway** - Single entry point for all services with authentication, routing, and load balancing.
- **Spring Security** - Implements authentication and authorization using JWT.
- **Spring Boot Admin** - Monitors and manages microservices in real-time.
- **Zipkin Server** - Distributed tracing for monitoring request flows.

## 🏗️ Tech Stack
- **Spring Boot**
- **Spring Cloud Netflix Eureka**
- **Spring Cloud Config**
- **Spring Cloud Gateway**
- **Spring Security**
- **Spring Boot Admin**
- **Zipkin (Distributed Tracing)**
- **MySQL/PostgreSQL (For persistence layer)**

## 🛠️ Microservices in the Project
| Service            | Port  | Description |
|--------------------|-------|-------------|
| **Eureka Server**  | `8761` | Service Registry for microservices |
| **Config Server**  | `8888` | Manages configurations of microservices |
| **API Gateway**    | `8080` | Routes requests to respective microservices |
| **Auth Service**   | `8081` | Handles authentication (JWT-based) |
| **User Service**   | `8082` | Manages user-related operations |
| **Order Service**  | `8083` | Handles orders and transactions |
| **Product Service**| `8084` | Manages product catalog |
| **Zipkin Server**  | `9411` | Monitors distributed tracing |
| **Admin Server**   | `9090` | Centralized monitoring of services |

## 🚀 Installation & Running Steps

### Prerequisites:
- **Java 17+**
- **Maven**
- **MySQL/PostgreSQL**

### 🏃 Steps to Run the Microservices

#### 1️⃣ Clone the Repository
```sh
git clone https://github.com/jayram0402/Spring-Boot-Microservice.git
cd Spring-Boot-Microservice

#### 2️⃣ Start the Eureka Service Registry
```sh
cd eureka-server
mvn spring-boot:run

#### 3️⃣ Start the Config Server
```sh
cd config-server
mvn spring-boot:run

#### 4️⃣ Start the API Gateway
cd api-gateway
mvn spring-boot:run

#### 5️⃣ Start the Microservices (Example: User Service)
'''sh
cd user-service
mvn spring-boot:run

#### 6️⃣ Start Zipkin Server (Optional - Requires Docker)
'''sh
docker run -d -p 9411:9411 openzipkin/zipkin

#### 7️⃣ Access Microservices:
Eureka Dashboard → http://localhost:8761
API Gateway → http://localhost:8080
Spring Boot Admin → http://localhost:9090
Zipkin Dashboard → http://localhost:9411

## 🔐 Security
JWT-based authentication is implemented using Spring Security.
API endpoints are secured, requiring authentication via tokens.

## 📊 Monitoring
Spring Boot Admin is used to track service health, logs, and uptime.
Zipkin provides distributed tracing for debugging.

## 📝 License
This project is open-source under the MIT License.

## 🔗 GitHub Repository: Spring Boot Microservice

## 👤 Author: Jayram Sharma


 

