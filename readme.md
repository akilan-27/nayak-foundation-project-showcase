# Nayak Foundation Portal

[![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white)](https://supabase.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)](https://vercel.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-444444?style=flat)](https://opensource.org/licenses/MIT)

A secure, full-stack NGO management platform developed for the Nayak Foundation to streamline volunteer registration, internship applications, and role-based administrative workflows.

[🌐 Explore Live Application](https://nayak-foundation-portal.vercel.app/)

---

# 📋 Table of Contents

* About the Project
* Problem Statement
* Solution
* Features
* User Roles
* Screenshots
* System Architecture
* Database Architecture
* Technology Stack
* Installation Guide
* Environment Variables
* Project Structure
* Application Workflow
* Authentication & Security
* Deployment Process
* Challenges Faced
* Lessons Learned
* Performance Optimizations
* Future Enhancements
* Contributors
* Author
* License

---

# 📖 About the Project

The Nayak Foundation Portal is a centralized web platform developed to digitize and simplify the process of managing volunteer and internship applications.

Traditionally, application management involved spreadsheets, emails, and manual record keeping, which often resulted in:

* Lost or duplicated information
* Delayed communication
* Administrative inefficiencies
* Lack of data security
* Difficult applicant tracking

This portal eliminates these challenges by providing a modern, role-based application management system with secure authentication and cloud-hosted infrastructure.

---

# 🚨 Problem Statement

Non-profit organizations frequently struggle with managing a growing number of volunteers and interns due to outdated manual processes.

The key challenges included:

* Manual application collection
* Unorganized applicant records
* No centralized database
* Difficulty tracking applications
* Lack of administrative controls
* Security concerns regarding applicant data

---

# 💡 Solution

The Nayak Foundation Portal provides:

✅ Centralized Application Management

✅ Secure Authentication System

✅ Volunteer Registration Portal

✅ Internship Registration Portal

✅ Administrative Dashboard

✅ Super Admin Control Panel

✅ Role-Based Access Control (RBAC)

✅ Cloud Database Integration

✅ Responsive User Experience

---

# ✨ Features

## 🔐 Authentication

* User Registration
* Secure Login
* Session Management
* Protected Routes
* Logout Functionality
* Password Recovery Support

## 👥 Volunteer Management

* Volunteer Registration Form
* Application Submission
* Data Validation
* Applicant Tracking

## 🎓 Internship Management

* Internship Application Form
* Educational Information Collection
* Experience Tracking
* Application Storage

## 📊 Admin Dashboard

* View Applications
* Review Applicant Information
* Filter Records
* Manage Volunteer Applications
* Manage Internship Applications

## ⚙️ Super Admin Dashboard

* User Management
* Role Assignment
* Admin Promotion
* Permission Control
* System Administration

## 📱 Responsive Design

* Mobile Friendly
* Tablet Compatible
* Desktop Optimized
* Cross-Browser Support

---

# 👤 User Roles

## General User

Users can:

* Register an account
* Login securely
* Submit volunteer applications
* Submit internship applications
* Access user-specific pages

---

## Administrator

Administrators can:

* Access Admin Dashboard
* Review submitted applications
* Manage volunteer records
* Manage internship records

---

## Super Administrator

Super Administrators can:

* Access all system features
* Manage user roles
* Promote users to administrators
* Oversee platform operations
* Manage permissions

---

# 📸 Screenshots

## Home Page

![Home Page](screenshots/home-page.png)

## Login Page

![Login Page](screenshots/login-page.png)

## Volunteer Registration

![Volunteer Registration](screenshots/volunteer-form.png)

## Internship Registration

![Internship Registration](screenshots/internship-form.png)

## Admin Dashboard

![Admin Dashboard](screenshots/admin-dashboard.png)

## Super Admin Panel

![Super Admin Panel](screenshots/super-admin-dashboard.png)

---

# 🏗 System Architecture

```text
User Browser
      │
      ▼
 React Frontend
      │
      ▼
 React Router
      │
      ▼
 Supabase Authentication
      │
      ▼
 PostgreSQL Database
      │
      ▼
 Row Level Security Policies
      │
      ▼
 Vercel Hosting
```

---

# 🗄 Database Architecture

## Main Tables

### Users

| Field      | Type      |
| ---------- | --------- |
| id         | UUID      |
| email      | String    |
| role       | String    |
| created_at | Timestamp |

### Volunteers

| Field     | Type   |
| --------- | ------ |
| id        | UUID   |
| name      | String |
| email     | String |
| phone     | String |
| interests | Text   |

### Internships

| Field          | Type   |
| -------------- | ------ |
| id             | UUID   |
| applicant_name | String |
| email          | String |
| qualification  | Text   |
| experience     | Text   |

---

# 🛠 Technology Stack

## Frontend

* React.js
* JavaScript (ES6+)
* Vite
* React Router DOM

## Styling

* Tailwind CSS
* CSS3

## Backend

* Supabase

## Database

* PostgreSQL

## Authentication

* Supabase Auth

## Animation

* Framer Motion

## Icons

* Lucide React

## Hosting

* Vercel

## Version Control

* Git
* GitHub

---

# ⚙ Installation Guide

## 1. Clone Repository

```bash
git clone https://github.com/your-username/nayak-foundation-portal.git
```

## 2. Navigate to Project

```bash
cd nayak-foundation-portal
```

## 3. Install Dependencies

```bash
npm install
```

## 4. Configure Environment Variables

Create a `.env` file:

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

## 5. Run Development Server

```bash
npm run dev
```

---

# 📂 Project Structure

```text
src/
│
├── assets/
│
├── components/
│   ├── Navbar
│   ├── Footer
│   ├── ProtectedRoute
│
├── pages/
│   ├── Home
│   ├── Login
│   ├── Register
│   ├── VolunteerForm
│   ├── InternshipForm
│   ├── Dashboard
│
├── services/
│   └── supabaseClient.js
│
├── hooks/
│
├── utils/
│
├── App.jsx
│
└── main.jsx
```

---

# 🔄 Application Workflow

### User Journey

1. User visits portal
2. User registers account
3. User logs in
4. User submits volunteer/internship application
5. Data stored securely in Supabase
6. Admin reviews applications
7. Super Admin manages users and permissions

---

# 🔒 Authentication & Security

Security measures implemented:

* Supabase Authentication
* Protected Routes
* Role-Based Access Control
* Row Level Security Policies
* Environment Variable Protection
* Session Persistence
* Secure API Communication

---

# 🚀 Deployment Process

## Development

Local Machine

↓

Git Repository

↓

GitHub Repository

↓

Vercel Deployment

↓

Production Environment

### Deployment Steps

1. Push code to GitHub
2. Connect repository to Vercel
3. Configure environment variables
4. Deploy application
5. Automatic updates on every push

---

# ⚡ Performance Optimizations

* Fast Vite Build System
* Component Reusability
* Efficient Routing
* Lazy Loading Opportunities
* Optimized Asset Management
* Cloud Database Integration

---

# 🧩 Challenges Faced

During development, several challenges were encountered:

* Implementing Role-Based Access Control
* Designing Secure Database Policies
* Managing Authentication States
* Protecting Admin Routes
* Creating Responsive Layouts
* Integrating Frontend with Supabase Backend

---

# 📚 Lessons Learned

This project strengthened my understanding of:

* React Architecture
* State Management
* Authentication Systems
* Database Design
* PostgreSQL
* Supabase Services
* Row Level Security
* API Integration
* Cloud Deployment
* GitHub Workflow

---

# 🔮 Future Enhancements

## Email Automation

* Application Status Emails
* Admin Notifications
* Welcome Emails

## Analytics Dashboard

* Volunteer Statistics
* Internship Trends
* Monthly Reports

## Data Export

* CSV Export
* Excel Reports
* PDF Reports

## User Profiles

* Resume Upload
* Skill Tracking
* Application History

## Advanced Features

* Dynamic Form Builder
* Multi-language Support
* SMS Notifications
* Activity Logs

---

# 🤝 Contributors

Developed as part of a web development project for the Nayak Foundation.

Contributions, suggestions, and improvements are welcome.

---

# 👨‍💻 Author

## Akilan

Aspiring Software Developer passionate about:

* Full Stack Development
* Web Technologies
* Database Design
* Open Source Development

### Connect With Me

GitHub: https://github.com/akilan-27

---

# ⭐ Support

If you found this project helpful, please consider giving it a star on GitHub.

---

# 📄 License

This project is licensed under the MIT License.

Copyright © 2026 Akilan

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files.

```
```
