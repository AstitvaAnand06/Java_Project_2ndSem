# 💳 Java Banking System with MySQL

This project is a simple banking system GUI built using Java Swing for frontend and MySQL for backend database. It supports account creation, deposit, withdrawal, and balance inquiry.

## 🧠 Key Features

- GUI using AWT/Swing
- MySQL database connectivity via JDBC
- Account type: Savings or Current
- Handles overdraft for current accounts (₹ -5000 limit)
- Modular, well-commented code

## 🏗 Database Setup

```sql
CREATE DATABASE bank_db;
USE bank_db;

CREATE TABLE accounts (
  accountNumber VARCHAR(20) PRIMARY KEY,
  holderName VARCHAR(50),
  accountType VARCHAR(20),
  balance DOUBLE
);
