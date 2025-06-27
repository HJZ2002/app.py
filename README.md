# 🧺 Laundry Management System

A secure web-based laundry management application built using **Flask**, **SQLite**, and **Bootstrap**.  
Designed to help laundry businesses manage orders, track status, and handle customer operations efficiently.

---

## 🔍 System Overview

This application provides an all-in-one platform for laundry business operations.  
Features include:

- Customer order tracking
- Status updates
- User authentication
- Responsive web interface

---

## 🔐 Security Features

The system follows industry-standard security practices:

- **Password Hashing:** Secure hashing with `werkzeug.security`
- **JWT Authentication:** Secure sessions with JSON Web Tokens
- **Token Expiration:** Configurable token timeouts
- **Authorization Headers:** API protection using Bearer tokens
- **Form Validation:** Input validation on both client & server
- **CORS Protection:** Cross-Origin Resource Sharing configured for safety
- **SQL Injection Prevention:** All DB queries use parameterized statements
- **XSS Protection:** Output sanitization before rendering templates
- **Session Management:** Secure handling of user sessions
- **Error Handling:** Minimal error output to avoid leaking system details
- **HTTPS Support:** HTTPS-compatible when deployed with valid certificates
- **Route Protection:** Authenticated routes secured via decorators
- **Token Verification:** Full validation of token integrity and signatures

---

## 🛠️ Development Tools

| Component     | Tech Used                   |
|---------------|-----------------------------|
| **Backend**   | Flask                       |
| **Database**  | SQLite (with prepared queries) |
| **Frontend**  | HTML5, CSS3, JavaScript, Bootstrap 5 |
| **Authentication** | JWT (JSON Web Tokens) |
| **HTTP Tunnel (Dev)** | LocalXpose          |

---
🚀 Running the Application
To get started with the application:

Install the required dependencies:

bash


pip install flask werkzeug pyjwt flask-cors
Ensure SQLite is available
SQLite is used as the database. Most systems come with it pre-installed. If not, install it based on your OS.

Run the application:

bash


python app.py
Access the web interface:
Open your browser and navigate to http://localhost:8000

🛠 Deployment
You can deploy the application using any of the following methods:

LocalXpose
For temporary public access during development or demonstration, use LocalXpose to expose your localhost via an HTTP tunnel.

Apache with mod_wsgi
Ideal for production environments using traditional server stacks. Configure WSGI to serve the Flask app via Apache.

Gunicorn or Waitress
Use these WSGI servers to serve the app in production-grade environments, especially when paired with a reverse proxy like Nginx.

🗃 Database Structure
Users Table

Manages user authentication and role-based access control (RBAC)

Stores hashed passwords securely using werkzeug.security

LaundryItems Table

Tracks laundry orders and item statuses

Contains customer information, timestamps, and order progress indicators
