\# Nayak Foundation Portal



A modern role-based web application developed for the Nayak Foundation to manage volunteer and internship registrations efficiently. The platform provides secure authentication, application tracking, and administrative controls through dedicated dashboards.



\## 🌐 Live Demo



\*\*Website:\*\* https://nayak-foundation-portal.vercel.app/



\---



\# 📖 Table of Contents



\* Overview

\* Problem Statement

\* Solution

\* Key Features

\* User Roles

\* System Architecture

\* Technology Stack

\* Database Design

\* Authentication \& Security

\* Project Workflow

\* Installation Guide

\* Environment Variables

\* Folder Structure

\* Screenshots

\* Challenges Faced

\* Lessons Learned

\* Future Improvements

\* Author



\---



\# 🎯 Overview



The Nayak Foundation Portal is a centralized platform that simplifies the process of managing volunteer and internship applications. Instead of handling applications manually through emails, spreadsheets, or paper forms, the system provides a secure and scalable solution where applicants and administrators can interact through a single portal.



The platform follows a Role-Based Access Control (RBAC) model, ensuring that each user only accesses features relevant to their responsibilities.



\---



\# 🚨 Problem Statement



Many non-profit organizations face challenges such as:



\* Managing applications manually

\* Tracking applicant information across multiple sources

\* Maintaining secure user records

\* Assigning administrative responsibilities

\* Managing growing applicant data



These issues often result in inefficiencies, data duplication, and delayed communication.



\---



\# 💡 Solution



The Nayak Foundation Portal addresses these challenges by providing:



\* Centralized application management

\* Secure authentication system

\* Role-based user permissions

\* Dedicated dashboards for administrators

\* Real-time database integration

\* Scalable cloud deployment



This enables the foundation to streamline operations while providing a professional application experience.



\---



\# ✨ Key Features



\## Authentication System



\* User Registration

\* Secure Login

\* Protected Routes

\* Session Management

\* Logout Functionality



\## Volunteer Registration



\* Online application submission

\* Personal information collection

\* Volunteer opportunity registration

\* Data validation



\## Internship Registration



\* Internship application forms

\* Educational information collection

\* Experience tracking

\* Application storage



\## Admin Dashboard



\* View all submitted applications

\* Manage volunteer registrations

\* Manage internship applications

\* Review applicant information

\* Track application records



\## Super Admin Panel



\* User Management

\* Role Management

\* Admin Creation

\* Permission Control

\* System Administration



\## Responsive Design



\* Mobile Friendly

\* Tablet Compatible

\* Desktop Optimized

\* Modern User Interface



\---



\# 👥 User Roles



\## General User



A general user can:



\* Create an account

\* Login securely

\* Apply for volunteer opportunities

\* Apply for internships

\* Access authorized pages



\## Administrator



An administrator can:



\* Access admin dashboard

\* View submitted applications

\* Manage volunteer records

\* Manage internship records



\## Super Administrator



A super administrator can:



\* Access all administrative features

\* Promote users to admin roles

\* Manage system users

\* Control permissions

\* Oversee platform operations



\---



\# 🏗 System Architecture



Frontend (React + Vite)



↓

React Router



↓

Supabase Authentication



↓

Supabase Database (PostgreSQL)



↓

Role-Based Access Control (RLS Policies)



↓

Vercel Deployment



\---



\# 🛠 Technology Stack



\## Frontend



\* React.js

\* Vite

\* JavaScript (ES6+)

\* React Router DOM



\## Styling



\* Tailwind CSS

\* Responsive Design Principles



\## Backend Services



\* Supabase Authentication

\* Supabase Database

\* Supabase API



\## Database



\* PostgreSQL



\## UI Enhancements



\* Framer Motion

\* Lucide React Icons



\## Hosting \& Deployment



\* Vercel



\## Version Control



\* Git

\* GitHub



\---



\# 🔐 Authentication \& Security



Security was one of the primary considerations while developing this platform.



Implemented measures include:



\* Secure user authentication using Supabase Auth

\* Protected frontend routes

\* Role-based authorization

\* Row Level Security (RLS) Policies

\* Environment Variable Protection

\* Session Handling

\* Restricted administrative access



\---



\# ⚙️ Project Development Workflow



\## Phase 1: Requirement Gathering



\* Identified foundation requirements

\* Defined user roles

\* Planned application flow



\## Phase 2: UI/UX Design



\* Designed navigation structure

\* Planned dashboard layouts

\* Created responsive interface designs



\## Phase 3: Frontend Development



\* Built reusable React components

\* Configured React Router

\* Developed forms and dashboards



\## Phase 4: Backend Integration



\* Configured Supabase project

\* Created database schema

\* Implemented authentication

\* Configured RLS policies



\## Phase 5: Testing



\* Authentication testing

\* Form validation testing

\* Role access testing

\* Responsive design testing



\## Phase 6: Deployment



\* Connected GitHub repository

\* Configured Vercel deployment

\* Added production environment variables

\* Published live application



\---



\# 📂 Folder Structure



src/



├── components/



├── pages/



├── hooks/



├── services/



├── utils/



├── assets/



├── App.jsx



└── main.jsx



\---



\# 🚀 Installation Guide



\## Clone Repository



git clone <repository-url>



\## Navigate To Project



cd nayak-foundation-portal



\## Install Dependencies



npm install



\## Start Development Server



npm run dev



\---



\# 🔑 Environment Variables



Create a .env file:



VITE\_SUPABASE\_URL=your\_supabase\_url



VITE\_SUPABASE\_ANON\_KEY=your\_supabase\_anon\_key



\---



\# 📸 Screenshots



Add screenshots of:



\* Landing Page

\* Login Page

\* Registration Page

\* Volunteer Form

\* Internship Form

\* Admin Dashboard

\* Super Admin Dashboard



\---



\# 🧩 Challenges Faced



During development, several challenges were encountered:



\* Configuring Role-Based Access Control

\* Implementing Supabase Authentication

\* Designing Row Level Security Policies

\* Managing Protected Routes

\* Maintaining Responsive UI Across Devices

\* Integrating Frontend with Backend Services



\---



\# 📚 Lessons Learned



This project helped strengthen my understanding of:



\* React Component Architecture

\* State Management

\* Client-Side Routing

\* Authentication Systems

\* Database Design

\* PostgreSQL

\* Supabase Services

\* Row Level Security

\* Deployment Pipelines

\* GitHub Collaboration Workflow



\---



\# 🔮 Future Improvements



\## Notifications



\* Email notifications for application updates

\* Admin alerts



\## Analytics



\* Volunteer participation reports

\* Internship analytics dashboard

\* Application statistics



\## Data Export



\* CSV Export

\* Excel Export

\* PDF Reports



\## Enhanced Profiles



\* Resume Upload

\* Skills Tracking

\* Application History



\## Advanced Administration



\* Dynamic Form Builder

\* Content Management System

\* Multi-language Support



\---



\# 👨‍💻 Author



Akilan



GitHub: https://github.com/your-github-username



LinkedIn: https://linkedin.com/in/your-linkedin-profile



\---



\# 📄 License



This project is licensed under the MIT License.



Feel free to use, modify, and distribute this project for educational and non-commercial purposes.



