# 🎓 CapTrack: Capstone Project Lifecycle Management System

CapTrack is a full-stack MERN web application that manages the lifecycle of university capstone projects in one place: finding teammates and a supervisor, tracking milestones, submitting deliverables, receiving feedback, and archiving finished work.

Built by **Group 5** for the Capstone Project course (CSE412) at **East West University**, Department of Computer Science and Engineering.

<img width="1874" height="881" alt="CapTrack dashboard" src="https://github.com/user-attachments/assets/3b607b44-6809-4629-8cb7-c6cebfed4acc" />

## 🌐 Live demo

| | Link |
|---|---|
| Frontend (Vercel) | https://frontend-scqb.vercel.app |
| Backend API (Render) | https://captrack-backend-3c36.onrender.com |
| Demo video | https://youtu.be/Hwu2flbv8Y8 |

> The backend runs on Render's free tier and sleeps when idle. The first request can take 30-50 seconds.

## 📦 Repositories

CapTrack is split into two repositories:

| Repo | Purpose |
|---|---|
| [frontend](https://github.com/SabikHossen07/frontend) | React + Vite single-page app |
| [captrack-backend](https://github.com/SabikHossen07/captrack-backend) | Express REST API with MongoDB |

This repository is the project landing page.

## ✨ Features

**Students**
- Registration and login restricted to university email domains, with JWT authentication and hashed passwords
- Dashboard with profile snapshot, project summary and activity feed
- Find teammates by skill, CGPA and availability
- Supervisor directory by research focus and open supervision slots, with direct supervision requests
- Collaboration feed for posting project ideas and applying to join groups
- Project workspace: overview, tasks and milestones, submissions, supervisor feedback, group chat and file sharing

**Supervisors**
- Dashboard of assigned groups, pending submissions and remaining supervision slots
- Approve or reject supervision requests
- Review milestone tasks, approve work, give feedback and extend deadlines
- Approve submissions or request revisions with notes

**Shared**
- Searchable project archive with abstracts, supervisor history and report/repository links
- Role-based access for students, supervisors and admins

## 🛠️ Tech stack

| Layer | Technology |
|---|---|
| Frontend | React, Vite, Tailwind CSS, Radix UI, Axios |
| Backend | Node.js, Express, Mongoose, JWT, bcryptjs |
| Database | MongoDB Atlas |
| Hosting | Vercel (frontend), Render (backend) |

## 🗂️ Data model

Users (roles: student, supervisor, admin), Projects, Supervision requests, Tasks, Submissions, Messages, Group files, Collaboration posts, Activity notifications, and Semesters.

## ⚙️ Run locally

```bash
git clone https://github.com/SabikHossen07/captrack-backend.git
git clone https://github.com/SabikHossen07/frontend.git
```

1. Set up the backend by following [captrack-backend](https://github.com/SabikHossen07/captrack-backend#readme).
2. Start the frontend:

```bash
cd frontend
npm install
npm run dev
```

The frontend points to the deployed backend by default. To use a local backend, change the `baseURL` in the `axios.create()` calls to `http://localhost:5000/api`.

## 👥 Team (Group 5)

- Md. Sabik Hossen
- Wasimul Bari Rahat

- Samira Akter

## 📄 License

Academic project, developed for coursework at East West University.
