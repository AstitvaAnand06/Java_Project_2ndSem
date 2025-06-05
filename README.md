# 🏦 Java GUI Banking System with MySQL Integration

A simple Banking System built using **Java Swing** for the GUI and **MySQL** for persistent data storage. This project demonstrates core Java concepts, JDBC integration, multi-threading with `SwingWorker`, and basic account management operations.

---

## 🚀 Features

- Create new bank accounts
- Deposit money
- Withdraw money with overdraft handling
- Show account balance and details
- Supports **Savings** and **Current** account types
- Database error handling and UI responsiveness via multithreading

---

## 🖥️ Tech Stack

- **Java (Swing + JDBC)**
- **MySQL**
- **SwingWorker** for background threading
- **Maven/Gradle (optional for dependency management)**

---

## 📦 Requirements

- Java JDK 11 or above
- MySQL Server installed and running
- MySQL JDBC Driver (Connector/J)
- IDE (IntelliJ, Eclipse, NetBeans) or terminal for compilation

---

## 🔧 Setup Instructions

### 🗃️ 1. Create the MySQL Database

Open MySQL and run:

```sql
CREATE DATABASE bank_db;

USE bank_db;

CREATE TABLE accounts (
    accountNumber VARCHAR(20) PRIMARY KEY,
    holderName VARCHAR(100),
    accountType VARCHAR(20),
    balance DOUBLE DEFAULT 0.0
);
