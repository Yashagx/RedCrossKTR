
# RedCrossKTR – Blood Bank Management System 🚑💻

**Live Demo:** [WEBAPP](https://yashagx.pythonanywhere.com/)

## 📝 Project Overview

**RedCrossKTR** is a **full-stack web application** developed for **SRM Global Hospitals** to digitize and streamline the **blood donation lifecycle**, **inventory management**, and **request workflows**. It addresses existing challenges caused by **manual data entry**, **lack of data traceability**, **communication gaps**, and **inefficient approval pipelines**.

The system implements **role-based access control (RBAC)**, real-time **CRUD operations**, and **transaction-safe inventory management**, ensuring **data consistency**, **availability**, and **integrity** across all modules.

## 🎯 Core Features

- **User Authentication and Authorization (RBAC)** using Django’s built-in `auth` system.
- **Donor Module**: Registration, health profiling, donation history.
- **Patient Module**: Request management with blood group matching.
- **Admin Module**: Centralized control panel for **inventory**, **approvals**, **user management**, and **real-time monitoring**.
- **Blood Stock Management**: Dynamic stock tracking using **SQL triggers**, **views**, and **aggregate queries**.
- **Notification Workflow**: Request status updates with **Admin-triggered approvals** and **real-time feedback**.
- **Data Validation and Integrity Constraints** at both **model** and **database** levels.

## 🏗️ Technology Stack

| Layer               | Technology                          |
|---------------------|-------------------------------------|
| Frontend            | HTML5, CSS3, JavaScript             |
| Backend Framework   | Django (Python)                     |
| Database            | SQLite3 (Relational DBMS)           |
| ORM                | Django ORM (Object Relational Mapping) |
| Server-Side Logic   | Django Views, Forms, Middleware     |
| Security            | Django Authentication, CSRF Protection, Password Hashing |
| Deployment          | Localhost / Development Server (Uvicorn / Django CLI) |

## 📊 Database Architecture & Design

- **Database Model**: **Normalized Relational Schema** (up to **BCNF**)
- **Tables/Entities**:
  - `auth_user`, `donar_donor`, `blood_stock`, `blood_bloodrequest`, `patient_patient`
- **Key Concepts Applied**:
  - **ER Modeling**
  - **Normalization (1NF → BCNF)**
  - **Primary and Foreign Keys**
  - **Cascade Operations**
  - **SQL Triggers, Views, Cursors**
  - **Transactional Integrity** with **ACID Compliance**

## 🧱 Backend Workflow Details

- **Django Models**: Abstract the database layer with **model classes** and **querysets**.
- **Custom Views**: Handle HTTP requests, implement **business logic**, and connect with templates.
- **Forms and Validation**: Django Form classes ensure **server-side data validation**.
- **Database Migrations**: Managed using Django’s **migration framework** (`makemigrations`, `migrate`).
- **Custom SQL Queries**: Implemented for **complex operations**, like **aggregations**, **search filters**, and **inventory updates**.
- **Concurrency Management**: Row-level locking using **transactions** and **atomic operations**.
- **Triggers & Functions**: Automatic stock updates on blood donation or approval events.

## 📈 Query & Data Manipulation Operations

- **DML (Data Manipulation Language)**:  
  - `INSERT`, `UPDATE`, `DELETE`, `SELECT`
- **DDL (Data Definition Language)**:  
  - Table creation scripts
- **Advanced SQL Operations**:
  - **Views**
  - **Stored Functions**
  - **Triggers for Real-Time Stock Sync**
  - **Cursors for Automated Reporting**

## ✅ Achievements and Impact

- **Reduced Manual Errors** with automated workflows.
- **Improved Blood Availability Visibility** through real-time dashboards.
- **Streamlined Approval Process** for donation and request management.
- **Ensured Data Security and Integrity** via Django’s built-in protection mechanisms.
- **Enabled Scalability and Maintainability** using modular MVC design patterns.

## 🛡️ Security Measures Implemented

- **Password Hashing** (PBKDF2 with salt)
- **CSRF Protection** on forms
- **SQL Injection Prevention** through Django ORM
- **Role-Based Permission Checks**
- **Data Access Restrictions** at the view level
- **Database Integrity Constraints** at the schema level

## 🚀 Future Scope and Enhancements

- **Twilio / SMTP Email Integration** for donor and admin notifications.
- **Mobile App Companion** (React Native / Flutter) for remote donor access.
- **AI-Driven Demand Forecasting** using historical request patterns.
- **Integration with Hospital EMR/EHR Systems** for unified patient care.
- **Blockchain-based Donation Traceability** for end-to-end transparency.

## 👨‍💻 Team Members

- **Yash Agarwal** – RA2311033010055  
- **Aaniya Jain** – RA2311033010057  

> *Department of Computational Intelligence, SRM Institute of Science and Technology, Kattankulathur.*

## 👨‍🏫 Project Guide

**Dr. R. Babu**  
Associate Professor  
Department of Computational Intelligence  
SRM IST
