# 📈 Stock Trading Simulation Platform

A **microservices-based backend system** that simulates real-world stock trading workflows including order placement, trade execution, portfolio updates, and wallet settlement.

---

## 🧱 Architecture

```
User Service → Order Service → Matching Engine → Portfolio Service
        ↑                                              ↓
        └──────────── Wallet Updates (User Service) ───┘
```

---

## 🚀 Services

### 🔹 User Service

Handles authentication and wallet balance management
👉 https://github.com/Vipul-Singh11/User-Service

---

### 🔹 Order Service

Handles BUY/SELL order placement and sends orders to the matching engine
👉 https://github.com/Vipul-Singh11/Order-Service

---

### 🔹 Matching Engine

Core trading engine that matches orders using price-time priority and executes trades
👉 https://github.com/Vipul-Singh11/Matching-Engine-Service

---

### 🔹 Portfolio Service

Updates user holdings after trade execution and ensures idempotency
👉 https://github.com/Vipul-Singh11/Portfolio-Service

---

### 🔹 Stock Price Service

Provides stock prices using Redis (used for portfolio valuation)
👉 https://github.com/Vipul-Singh11/Stock-Price-Service

---

## 🔄 Trade Flow

1. User places BUY/SELL order
2. Order Service forwards it to Matching Engine
3. Matching Engine matches orders and executes trade
4. Portfolio Service updates holdings
5. User Service updates wallet balances

---

## ⚙️ Tech Stack

* Java
* Spring Boot
* MySQL
* Redis
* REST APIs

---

## 🧠 Key Concepts Implemented

* Microservices Architecture
* In-memory Order Book
* Price-Time Priority Matching
* Idempotent Trade Processing
* Inter-service Communication
* Transaction Handling

---

## 📌 Note

Each service is maintained as an independent repository.
This repository serves as a central documentation hub for the system.

---

## 🚀 Future Improvements

* Kafka for event-driven architecture
* Circuit breakers (Resilience4j)
* Distributed transaction handling
* Frontend dashboard (React)

---

## 👨‍💻 Author

**Vipul Singh**
GitHub: https://github.com/Vipul-Singh11

---
