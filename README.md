# 📈 Stock Trading Simulation Platform

A full-stack **Stock Trading Simulation Platform** built using a **microservices architecture** that simulates real-world stock trading workflows including order placement, order matching, trade execution, portfolio management, wallet settlement, and market visualization.

---

## 🏗️ System Architecture

```text
Frontend (React)
       │
       ▼
User Service ↔ Order Service ↔ Matching Engine
      ▲              │               │
      │              ▼               ▼
      └──── Portfolio Service ← Stock Price Service
```

---

## 🚀 Services

### 🔹 User Service

Handles:

* User Registration & Login
* JWT Authentication
* Wallet Balance Management
* Reserved Balance Tracking
* Fund Reservation & Settlement

Repository:
👉 https://github.com/Vipul-Singh11/User-Service

---

### 🔹 Order Service

Handles:

* BUY / SELL Order Placement
* Order Validation
* Order Cancellation
* Partial Fill Handling
* Order Status Management
* Fund and Share Reservation Logic

Repository:
👉 https://github.com/Vipul-Singh11/Order-Service

---

### 🔹 Matching Engine Service

Core trading engine responsible for:

* Price-Time Priority Matching
* In-Memory Order Book
* Trade Execution
* Partial Trade Processing
* Order Book Visualization Support

Repository:
👉 https://github.com/Vipul-Singh11/Matching-Engine-Service

---

### 🔹 Portfolio Service

Handles:

* Portfolio Holdings
* Trade History
* Portfolio Summary
* Share Reservation Management
* Idempotent Trade Processing

Repository:
👉 https://github.com/Vipul-Singh11/Portfolio-Service

---

### 🔹 Stock Price Service

Provides:

* Stock Master Data
* Current Market Prices
* Portfolio Valuation Support
* Redis-Based Price Caching

Repository:
👉 https://github.com/Vipul-Singh11/Stock-Price-Service

---

### 🔹 Frontend Application

Modern React-based trading dashboard providing:

* Authentication
* Portfolio Management
* Order Placement
* Trade History
* Order Book Visualization
* Stock Market Dashboard
* Portfolio Analytics
* Interactive Charts

Repository:
👉 https://github.com/Vipul-Singh11/Stock-Trading-Frontend

---

## 🔄 Trade Execution Flow

1. User places a BUY or SELL order.
2. Order Service validates the request.
3. Funds or shares are reserved.
4. Order is forwarded to the Matching Engine.
5. Matching Engine matches orders using price-time priority.
6. Trade execution occurs.
7. Portfolio Service updates holdings and trade history.
8. User Service settles wallet balances.
9. Frontend reflects updated portfolio and order status.

---

## 📊 Frontend Features

### Dashboard

* Wallet Balance
* Reserved Balance
* Available Balance
* Portfolio Summary
* Recent Trades
* Performance Cards

### Portfolio

* Holdings Overview
* Available Quantity
* Reserved Quantity
* Portfolio Allocation Charts
* Portfolio Distribution Visualizations

### Stocks

* Stock Listings
* Company Information
* Current Market Prices
* Interactive Price Charts
* Search & Filtering

### Orders

* Place BUY / SELL Orders
* Cancel Pending Orders
* View Order Status
* Partial Fill Tracking

### Trade History

* Trade Tracking
* Search & Filtering
* Sortable History Table

### Order Book

* Live Buy/Sell Order Visualization
* Best Bid / Best Ask Display
* Auto Refresh Support

---

## ⚙️ Tech Stack

### Backend

* Java
* Spring Boot
* Spring Security
* JWT Authentication
* MySQL
* Redis
* REST APIs
* Maven

### Frontend

* React JS
* Vite
* Material UI
* Axios
* React Router
* Recharts

---

## 🧠 Key Concepts Implemented

### Backend

* Microservices Architecture
* JWT Authentication
* Inter-Service Communication
* Reservation-Based Trading
* In-Memory Matching Engine
* Price-Time Priority Matching
* Trade Settlement
* Portfolio Management
* Transaction Handling
* Idempotent Processing

### Frontend

* Protected Routes
* Context-Based Authentication
* Reusable Components
* Dashboard Analytics
* Data Visualization
* Interactive Charts
* Responsive UI Design

---

## 📈 Implemented Trading Features

✅ User Authentication

✅ Wallet Management

✅ Fund Reservation

✅ Share Reservation

✅ Order Placement

✅ Order Cancellation

✅ Partial Fills

✅ Order Matching

✅ Trade Execution

✅ Portfolio Updates

✅ Trade History

✅ Portfolio Analytics

✅ Order Book Visualization

✅ Interactive Stock Dashboard

---

## 🔮 Future Enhancements

* Market Orders
* Kafka-Based Event Streaming
* Real-Time WebSocket Updates
* Circuit Breakers (Resilience4j)
* Docker & Kubernetes Deployment
* Historical Stock Price Storage
* Advanced Trading Analytics
* Notifications & Alerts

---

## 👨‍💻 Author

**Vipul Singh**

GitHub:
https://github.com/Vipul-Singh11
