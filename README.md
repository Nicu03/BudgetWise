# BudgetWise

**BudgetWise** is a service-oriented budgeting application designed for efficient personal finance management. This application utilizes **Windows Communication Foundation (WCF)** for its service layer and leverages **Docker** for containerization, ensuring a modern and scalable architecture.

---

## 📚 Project Overview

The goal of this project is to demonstrate the integration of **Windows Communication Foundation (WCF)** in a service-oriented architecture. BudgetWise enables users to:
- Manage and track their income and expenses.
- Set budgets and receive alerts.
- Generate reports for better financial insight.

---

## 🛠 Features

1. **User Authentication and Authorization**
   - Secure login and registration.
   - Role-based access control (e.g., admin and standard users).

2. **Income and Expense Management**
   - Add, update, delete, and view income and expense records.
   - Categorize transactions for better tracking.

3. **Budget Planning and Tracking**
   - Set budget goals and monitor spending.
   - Get alerts when spending exceeds budget limits.

4. **Reporting and Analytics**
   - Visualize financial data with graphs and charts.
   - Export reports in various formats.
  
---

## 🏗 Architecture

The application follows a **Service-Oriented Architecture (SOA)** using **WCF** for communication between services. The key components include:
- **UI**: The front-end interface for user interaction.
- **WCF Services**: The back-end service layer managing business logic and data communication.
- **Database**: A SQL Server database for storing user data and financial records.

The entire project is containerized using **Docker** to simplify deployment and ensure consistency across environments.

---

## 📦 Technology Stack

- **C# / .NET Framework**: For building WCF services.
- **SQL Server**: For data storage.
- **Docker**: For containerization and easy deployment.
- **WCF (Windows Communication Foundation)**: For creating and consuming web services.
- **GitHub Actions**: For continuous integration and deployment.

---
