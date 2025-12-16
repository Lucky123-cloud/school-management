````md
# JKAUT School Management System

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
````

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

---

## Project Overview

The **JKAUT School Management System** is a modern, minimalistic web-based platform designed to manage and streamline academic and administrative activities within a school environment. The system focuses on clarity, real-world relationships, and role-based access while remaining intentionally simple for learning and presentation purposes.

---

## Purpose of the System

This system provides a centralized platform where:

* Admins manage the overall school structure
* Teachers manage subjects, classes, homework, and announcements
* Students access their academic information
* Parents monitor their children’s academic progress and attendance

The platform mirrors real school workflows while maintaining a clean and minimal implementation.

---

## User Roles and Responsibilities

### Admins

Admins have full control over the system and can:

* Manage users (students, teachers, parents)
* Create and manage classes and subjects
* Assign teachers to subjects
* Enroll students into classes and subjects
* Oversee the overall school structure

---

### Teachers

Teachers are responsible for academic content and classroom management. They can:

* Teach multiple subjects
* Manage subjects they are assigned to
* Post homework and assignments
* Publish announcements
* Record and update student grades
* Track attendance for their classes

---

### Students

Students have access to their academic information and can:

* Enroll in multiple subjects
* View grades per subject
* Access homework and assignments
* Read announcements
* View attendance records
* See registered classes and subjects

---

### Parents

Parents act as supervisors of student progress. The system supports:

* Parents having multiple children enrolled
* Viewing each child’s:

  * Grades
  * Subjects and classes
  * Homework and announcements
  * Attendance records

Parents have read-only access to their children’s academic data.

---

## Core System Relationships

* A parent can have many students (children)
* A teacher can teach many subjects
* A student can enroll in many subjects
* A subject can have many students
* Grades, attendance, and homework are linked to students and subjects

These relationships are managed using **PostgreSQL** and **Prisma ORM** to ensure data integrity and clarity.

---

## Technology Stack

### Frontend

* Next.js (App Router)
* TypeScript
* Minimalistic UI focused on usability and clarity

### Backend & Database

* Prisma ORM for schema definition and relations
* PostgreSQL for robust relational data management
* API routes and server actions handled within Next.js

---

## Authentication & Authorization (Current Status)

Authentication and authorization are currently **bypassed** for development and presentation purposes.

* Login routes are placed under `PUBLIC_URL`
* This allows unrestricted access during development
* The team is actively learning and implementing AuthN and AuthZ using **Clerk**
* Authentication is not yet production-ready

This approach allows focus on core system logic and data relationships without unstable auth implementations.

---

## Design Philosophy

The system follows a minimalistic, learning-first approach:

* Clear role separation
* Strong relational data modeling
* Maintainable and readable code
* Scalable architecture for future enhancements
* Practical functionality over feature overload

---

## Development Status

* Core entities and relationships implemented
* Role-based behavior defined
* Authentication temporarily bypassed
* Optimized for presentation and learning
* Designed for future expansion

---

## Conclusion

The **JKAUT School Management System** demonstrates how modern web technologies can be used to build a structured, role-based application that reflects real-world school operations. While minimal by design, the system provides a strong foundation for future development and production readiness.

```
