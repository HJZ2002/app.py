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

