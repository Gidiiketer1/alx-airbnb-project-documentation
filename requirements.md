# Backend Requirement Specifications — ALX Airbnb Project

## Objective
This document outlines the functional and technical requirements for the key backend features of the Airbnb-like system.  
The backend is designed to handle user authentication, property management, and booking operations efficiently and securely.

---

## 1. User Authentication

### **Description**
Allows users to register, log in, and manage their accounts securely.

### **API Endpoints**
| Method | Endpoint | Description |
|--------|-----------|--------------|
| `POST` | `/api/auth/register/` | Register a new user |
| `POST` | `/api/auth/login/` | Authenticate user and generate token |
| `GET` | `/api/auth/profile/` | Retrieve user profile (authorized users only) |
| `PUT` | `/api/auth/profile/update/` | Update user details |

### **Input / Output**
**Input:**  
```json
{
  "username": "gideon",
  "email": "gideon@example.com",
  "password": "SecurePass123"
}
