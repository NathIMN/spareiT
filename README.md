# 🚗 SpareiT - Automotive Parts E-Commerce Platform

A comprehensive multi-user web application for automotive spare parts management, connecting customers, suppliers, support agents, and administrators in a seamless marketplace.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![JSP](https://img.shields.io/badge/JSP-Servlets-blue)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat&logo=bootstrap&logoColor=white)

## 📋 Overview

SpareiT is a full-stack e-commerce platform designed to streamline automotive spare parts procurement and management. Built with Java EE technologies, it features intelligent vehicle compatibility matching, real-time inventory tracking, and role-based workflows for different user types.

**SLIIT Year 2 Semester 1 - Object-Oriented Programming Group Project**

## ✨ Key Features

### 🔐 Multi-Role Authentication
- **Customers**: Browse parts, manage cart, submit inquiries
- **Suppliers**: Handle restock requests, view registered items
- **Agents**: Manage customer inquiries and provide support
- **Admin**: Full inventory management and system oversight

### 🔍 Smart Search & Compatibility
- Advanced filtering by vehicle make, model, and year
- Dynamic compatibility matching system
- Real-time stock availability validation
- Category-based parts browsing

### 🛒 Shopping Cart Management
- Persistent cart with session management
- Real-time quantity updates
- Stock validation before checkout
- Cart count tracking across sessions

### 📦 Inventory Management
- Complete CRUD operations for parts catalog
- Multi-vehicle compatibility assignment
- Dynamic form generation for complex data entry
- Admin dashboard for system control

### 💬 Customer Support System
- Inquiry submission with vehicle specifications
- Urgency level and inquiry type categorization
- Agent response and status tracking
- Customer inquiry history

## 🛠️ Technologies

- **Backend**: Java EE, JSP/Servlets, JDBC
- **Frontend**: HTML5, CSS3, Bootstrap 5, JavaScript
- **Database**: MySQL
- **Server**: Apache Tomcat
- **Architecture**: MVC Pattern with Three-Tier Architecture

## 📁 Project Structure

```
src/main/
├── java/
│   ├── model/          # Entity classes (Customer, Item, Cart, etc.)
│   ├── service/        # Business logic controllers
│   ├── servlet/        # Request handlers
│   └── util/           # Database utilities
└── webapp/
    ├── admin/          # Admin dashboard pages
    ├── Customer/       # Customer interface
    ├── Inquiry/        # Inquiry management
    ├── supplier/       # Supplier workflows
    └── Partials/       # Reusable components
```

## 🚀 Getting Started

### Prerequisites
- JDK 8 or higher
- Apache Tomcat 9+
- MySQL 5.7+
- IDE (Eclipse/IntelliJ IDEA)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/NathIMN/spareiT.git
   ```

2. **Database Setup**
   - Import `spareiT.sql` into your MySQL server
   - Update database credentials in `application.properties`

3. **Configure Tomcat**
   - Deploy the project to your Tomcat server
   - Ensure all required libraries are in `WEB-INF/lib`

4. **Run the Application**
   - Start Tomcat server
   - Access at `http://localhost:8080/spareiT`

## 👥 Default Login Credentials

| Role | Email | Password |
|------|-------|----------|
| Customer | nadshrio@gmail.com | 123 |
| Admin | nath@gmail.com | nath |
| Supplier | alice@supplyco.com | alice123 |
| Agent | alice@example.com | password123 |

## 🏗️ Architecture

**Three-Tier MVC Architecture:**
- **Presentation Layer**: JSP pages with Bootstrap UI
- **Business Logic Layer**: Service controllers and interfaces
- **Data Access Layer**: JDBC with prepared statements

**OOP Principles Applied:**
- Inheritance hierarchies for user roles
- Interface implementation for service contracts
- Encapsulation across model entities
- Polymorphism in user authentication
