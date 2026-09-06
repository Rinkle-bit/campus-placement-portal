# campus-placement-portal
# 🎓 CampusConnect — Campus Placement Portal

> **A full-stack web application designed to simplify and digitize the campus placement process for students and placement-cell administrators.**

CampusConnect is a modern **Campus Placement Management System** that provides a centralized platform where students can discover job opportunities, apply for suitable positions, and track their applications, while administrators can manage job openings and monitor placement activity through a dedicated dashboard.

---

## 🚀 Why CampusConnect?

Traditional placement processes often involve spreadsheets, notices, forms, and manual application tracking.

**CampusConnect brings these activities into one centralized platform**, making the placement workflow more organized, accessible, and efficient.

### 🎯 Key Goals

* Simplify job discovery for students
* Provide a seamless online application process
* Track student applications digitally
* Give placement administrators centralized control
* Provide useful placement statistics through an admin dashboard
* Implement secure authentication and role-based access

---

## ✨ Key Features

### 👨‍🎓 Student Portal

* Student registration and secure login
* Browse available job opportunities
* View company, location, package, description and deadline
* Apply to jobs with a single click
* Track submitted applications

### 🛠️ Admin Dashboard

* Secure administrator authentication
* View placement statistics
* Monitor registered students
* Monitor job opportunities and applications
* Create new job openings
* Delete outdated job postings
* View recent application activity

### 🔐 Authentication & Security

* JWT-based authentication
* Role-based authorization
* Password hashing using bcrypt
* Protected student and admin routes
* Environment-based configuration for sensitive secrets

---

## 🧑‍💻 Tech Stack

| Layer          | Technologies                        |
| -------------- | ----------------------------------- |
| Frontend       | React 19, Vite                      |
| Backend        | Node.js, Express.js                 |
| Database       | SQLite, better-sqlite3              |
| Authentication | JSON Web Token (JWT)                |
| Security       | bcryptjs                            |
| API            | RESTful APIs                        |
| Development    | Concurrent frontend + backend setup |

---

## 🏗️ Architecture

```text
                    ┌─────────────────────┐
                    │      React UI       │
                    │      + Vite         │
                    └──────────┬──────────┘
                               │
                         REST API Calls
                               │
                    ┌──────────▼──────────┐
                    │   Node.js + Express │
                    │      Backend API    │
                    └──────────┬──────────┘
                               │
                  ┌────────────▼────────────┐
                  │       SQLite DB         │
                  │ Users | Jobs | Apps     │
                  └─────────────────────────┘

              Authentication → JWT + bcrypt
```

---

## 📂 Project Structure

```text
campus-placement-portal/
│
├── server/
│   ├── index.js
│   └── placement.db
│
├── src/
│   ├── main.jsx
│   └── style.css
│
├── .env.example
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

---

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/campus-placement-portal.git
cd campus-placement-portal
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file using `.env.example` and add a secure JWT secret:

```env
JWT_SECRET=your_secure_secret
```

### 4. Start the application

```bash
npm run dev
```

The frontend and backend will start together.

---

## 🔑 Demo Credentials

### Student

```text
Email: student@college.edu
Password: student123
```

### Admin

```text
Email: admin@college.edu
Password: admin123
```

> ⚠️ Demo credentials are provided only for local testing. Use secure credentials and secrets in production.

---

## 📊 Database Design

CampusConnect uses SQLite with three core entities:

```text
Users
 ├── Student
 └── Admin

Jobs
 ├── Job Title
 ├── Company
 ├── Location
 ├── Package
 ├── Description
 └── Deadline

Applications
 ├── Student
 ├── Job
 └── Application Date
```

This structure allows the system to connect students with job opportunities and maintain application history efficiently.

---

## 💡 What I Learned

Building CampusConnect helped me strengthen my understanding of:

* Full-stack web application development
* React component-based development
* REST API design
* Node.js & Express backend development
* SQL database design and CRUD operations
* JWT authentication
* Password hashing and security practices
* Role-based authorization
* Frontend-backend integration
* Environment variable management
* Building a real-world workflow instead of isolated features

---

## 🔮 Future Enhancements

The project can be extended with:

* 📄 Resume upload and management
* 📧 Email notifications
* 🏢 Company/recruiter accounts
* 📅 Interview scheduling
* 🔎 Advanced job filtering and search
* 📈 Advanced placement analytics
* 🔔 Application status notifications
* ☁️ PostgreSQL-based production database
* 📱 Improved mobile responsiveness

---

## 🌟 Project Highlights

**CampusConnect demonstrates practical implementation of:**

`React` • `Node.js` • `Express.js` • `SQLite` • `REST API` • `JWT` • `bcrypt` • `CRUD` • `Role-Based Access Control`

> **Built to transform a manual campus placement workflow into a centralized digital experience.**

---

## 👩‍💻 Developer

**Rinkle**
B.Tech Computer Science & Engineering Student

Interested in **Software Development | Full-Stack Development | Web Technologies**

---

⭐ If you find this project useful, consider giving the repository a star!
