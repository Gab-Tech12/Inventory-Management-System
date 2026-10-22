# 📦 Inventory Management System (Sistema de Gerenciamento de Estoque)

A robust Java backend application designed to manage product inventories, demonstrating core Object-Oriented Programming (OOP) principles, clean layered architecture, and direct database interaction using JDBC.

---

## 🚀 Technologies & Tools

* **Language:** Java 17+
* **Database:** PostgreSQL / MySQL
* **Persistence:** JDBC (`java.sql.*`)
* **Build Tool:** Apache Maven
* **IDEs:** IntelliJ IDEA / VS Code

---

## 🎯 Key Features

- **Create:** Register new products with validation for price and stock levels.
- **Read:** Fetch all products or search by unique product ID.
- **Update:** Modify existing product attributes (name, quantity, price).
- **Delete:** Remove products securely from the database.
- **SQL Injection Prevention:** Implemented using `PreparedStatement`.
- **Resource Management:** Automatic connection closing via `try-with-resources`.

---

## 🏗️ Architecture & Project Structure

The project follows a Layered Architecture to separate concerns and maintain clean, scalable code:

```text
src/main/java/com/gabriel/estoque/
├── config/              # Database connection management (ConnectionFactory)
├── model/               # Domain entities (Produto)
├── dao/                 # Data Access Object pattern (Interface & Implementation)
└── Main.java            # Main application entry point & CLI interaction
