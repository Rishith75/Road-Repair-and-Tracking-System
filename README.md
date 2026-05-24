# Road Repair and Tracking System

A full-stack road maintenance and complaint management platform designed to streamline complaint registration, resource allocation, work scheduling, and repair tracking for municipal road infrastructure.

Developed as part of the Software Engineering Laboratory under Prof. Sourangshu Bhattacharya at IIT Kharagpur, this system enables coordinated interaction between clerks, supervisors, and administrators through a centralized workflow management platform.

---

# Features

## Complaint Management
- Citizens’ road complaints handled through clerk workflows
- Complaint creation, tracking, and status management
- Complaint lifecycle:
  - New
  - Pending
  - Ongoing
  - Completed

## Resource Allocation
- Supervisors can:
  - estimate required materials
  - assign workers
  - specify repair duration
  - set work priority

## Automated Work Scheduling
- Priority-based scheduling system
- Resource-aware task allocation
- Dynamic work queue generation based on:
  - urgency
  - available workers
  - material constraints

## Real-Time Monitoring
- Live work statistics and tracking
- Status dashboards for administrators
- Progress monitoring for supervisors

## User Management
Role-based access control for:
- Clerk
- Supervisor
- Administrator

Supports:
- authentication
- profile updates
- secure password modification

## Notifications and Alerts
- Real-time alerts for workflow updates
- Push notifications for status changes
- Scheduling and assignment updates

---

# Tech Stack

## Frontend
- React.js
- Chart.js
- HTML/CSS
- JavaScript

## Backend
- Node.js
- Express.js

## Database
- MongoDB

## Testing & Deployment
- End-to-end workflow testing
- REST API integration
- Deployment-ready architecture

---

# System Workflow

```text
Complaint Registration
          ↓
Supervisor Resource Estimation
          ↓
Priority Assignment
          ↓
Automated Work Scheduling
          ↓
Resource Allocation
          ↓
Work Execution
          ↓
Completion Tracking & Statistics
```

---

# Project Architecture

```text
Frontend (React + Chart.js)
              ↓
REST APIs (Express.js)
              ↓
Business Logic Layer
              ↓
MongoDB Database
```

---

# Functional Modules

## Clerk Module
- Register road complaints
- Track complaint status
- Manage complaint records
- Update profile information

## Supervisor Module
- Review incoming complaints
- Estimate required resources
- Assign priorities and repair durations
- Mark repairs as completed

## Administrator Module
- Update city-wide resources
- Generate and update work schedules
- Monitor ongoing works
- Analyze repair statistics

---

# Database Design

MongoDB collections were designed for:
- Users
- Complaints
- Resource inventory
- Work schedules
- Notifications
- Repair statistics

The backend supports efficient querying and workflow tracking using RESTful APIs.

---

# Key Engineering Concepts

- REST API design
- Role-based authentication
- Scheduling and prioritization algorithms
- Resource-constrained task allocation
- Real-time workflow tracking
- Full-stack state management
- Scalable backend architecture

---

# Sample Workflow

## Complaint Registration
A clerk registers a road repair complaint containing:
- location
- issue details
- urgency

## Resource Planning
The supervisor:
- estimates required workers/materials
- sets priority
- specifies expected repair time

## Schedule Generation
The administrator updates the work schedule, allocating:
- workers
- materials
- timelines

based on resource availability and task priority.

## Completion Tracking
Supervisors mark completed repairs, updating:
- complaint status
- city statistics
- ongoing work dashboards

---

# Setup Instructions

## Clone Repository

```bash
git clone <repository-url>
cd road-repair-tracking-system
```

---

# Backend Setup

## Install Dependencies

```bash
cd backend
npm install
```

## Configure Environment Variables

Create a `.env` file:

```env
MONGO_URI=your_mongodb_connection
PORT=5000
JWT_SECRET=your_secret_key
```

## Start Backend Server

```bash
npm start
```

---

# Frontend Setup

## Install Dependencies

```bash
cd frontend
npm install
```

## Start Frontend

```bash
npm start
```

---

# Future Improvements

- GIS/Map integration
- Mobile application support
- Predictive maintenance using ML
- Route optimization for repair crews
- Cloud-native deployment
- Real-time GPS tracking

---

# Team Contribution

Developed as part of a team project for Software Engineering coursework at IIT Kharagpur.

My contributions included:
- Backend API development using Node.js and Express
- MongoDB schema design
- Complaint workflow implementation
- Scheduling and prioritization logic
- REST API integration
- Frontend feature integration
- Real-time statistics and alerts

---

# Learning Outcomes

This project provided practical experience with:
- full-stack application development
- scalable backend engineering
- RESTful API design
- workflow automation
- scheduling systems
- MongoDB schema modeling
- frontend-backend integration
- software engineering lifecycle practices

---

# Acknowledgements

Developed as part of the Software Engineering Laboratory under Prof. Sourangshu Bhattacharya at IIT Kharagpur.
