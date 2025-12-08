# SpareiT - Online Auto Spare Parts Management System

A comprehensive multi-user web application for automotive spare parts management, connecting customers, suppliers, support agents, and administrators on a unified platform.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![JSP](https://img.shields.io/badge/JSP-Servlets-blue)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat&logo=bootstrap&logoColor=white)

## Overview

SpareiT is an online auto spare parts management system developed to streamline the process of buying and selling spare parts online. By automating key operations and facilitating seamless management and distribution, SpareiT aims to revolutionize the spare parts industry by significantly increasing overall efficiency.

Built with Java EE technologies, the platform features intelligent vehicle compatibility matching, real-time inventory tracking, and role-based workflows designed to ensure optimal performance for all user types.

**SLIIT Year 2 Semester 1 - Object-Oriented Programming Group Project**

## Key Features

### Multi-Role System Architecture

**Customers**
- Self-registration and secure authentication
- Browse and search spare parts with advanced filtering
- Shopping cart management with real-time updates
- Checkout and order processing
- Submit inquiries for out-of-stock or unlisted items
- View inquiry status and agent responses

**Suppliers**
- Monitor current inventory stock levels
- Submit restock requests for specialized parts
- View registered items and request status
- Payment processing through the system
- Track approved and pending requests

**Customer Support Agents**
- Handle customer inquiries on availability
- Act as a bridge between customers and suppliers
- Contact suppliers to verify brand availability
- Recommend alternative brands when needed
- Process after-sale operations (warranty checks, returns)
- Provide responses and update inquiry status

**Administrators**
- Review and authorize supplier applications for new parts
- Approve or reject restock requests based on inventory levels
- Full CRUD operations on parts catalog
- Remove faulty or discontinued items
- Maintain inventory integrity and quality control
- System oversight and user management

### Technical Features
- Advanced vehicle compatibility matching (Make, Model, Year)
- Dynamic search with cascading filters
- Real-time stock availability validation
- Session-based persistent shopping cart
- Multi-vehicle compatibility assignment per part
- Inquiry management with urgency levels and categorization

## Technologies

- **Backend**: Java EE, JSP/Servlets, JDBC
- **Frontend**: HTML5, CSS3, Bootstrap 5, JavaScript
- **Database**: MySQL
- **Server**: Apache Tomcat
- **Architecture**: MVC Pattern with Three-Tier Architecture

## Project Structure

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

## Getting Started

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

## Default Login Credentials

| Role | Email | Password |
|------|-------|----------|
| Customer | nadshrio@gmail.com | 123 |
| Admin | nath@gmail.com | nath |
| Supplier | alice@supplyco.com | alice123 |
| Agent | alice@example.com | password123 |

## Screenshots

### Home Page
![Home Page](screenshots/Screenshot%202025-11-30%20at%2017-04-19%20spareiT%20Home.jpeg)

<table>
  <tr>
    <td width="50%">
      <h3>Search Results</h3>
      <img src="screenshots/FireShot%20Capture%20013%20-%20spareiT%20-%20Search%20Results%20-%20localhost.jpeg" alt="Search Results" width="100%">
    </td>
    <td width="50%">
      <h3>Shopping Cart</h3>
      <img src="screenshots/FireShot%20Capture%20015%20-%20spareiT%20-%20Shopping%20Cart%20-%20localhost.jpeg" alt="Shopping Cart" width="100%">
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>Admin Parts Catalog</h3>
      <img src="screenshots/FireShot Capture 020 - Auto Parts Catalog - localhost.jpeg" alt="Admin Parts Catalog" width="100%">
    </td>
    <td width="50%">
      <h3>Item Details Management</h3>
      <img src="screenshots/Screenshot%202025-11-30%20at%2017-04-03%20Item%20Details%20-%20Auto%20Parts.jpeg" alt="Item Details" width="100%">
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>Inquiry Management</h3>
      <img src="screenshots/FireShot%20Capture%20017%20-%20View%20_%20Update%20Inquiry%20-%20localhost.jpeg" alt="Inquiry Management" width="100%">
    </td>
    <td width="50%">
      <h3>Restock Requests</h3>
      <img src="screenshots/FireShot%20Capture%20016%20-%20View%20Restock%20Requests%20-%20localhost.jpeg" alt="Restock Requests" width="100%">
    </td>
  </tr>
</table>

## Architecture

**Three-Tier MVC Architecture:**
- **Presentation Layer**: JSP pages with Bootstrap UI
- **Business Logic Layer**: Service controllers and interfaces
- **Data Access Layer**: JDBC with prepared statements

**OOP Principles Applied:**
- Inheritance hierarchies for user roles
- Interface implementation for service contracts
- Encapsulation across model entities
- Polymorphism in user authentication
