# Full-Stack Development Internship – Final Project Submission

<p align="center">
  <h1 align="center">Full-Stack Development Projects</h1>
  <p align="center">
    A collection of two full-stack applications developed as part of the Full-Stack Development internship, demonstrating modern web development, real-time collaboration, and practical software engineering.
  </p>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Track-Full--Stack%20Development-blue" alt="Full-Stack Development" />
  <img src="https://img.shields.io/badge/Projects-2-success" alt="Two Projects" />
  <img src="https://img.shields.io/badge/Status-Ready%20for%20Review-orange" alt="Ready for Review" />
  <img src="https://img.shields.io/badge/Repository-Public-brightgreen" alt="Public Repository" />
</p>

---

## 📌 Internship Information

| Detail | Information |
|---|---|
| Specialization Track | Full-Stack Development |
| Batch Start Date | 20 October 2026 |
| Project Deadline | 20 November 2026 |
| Estimated Effort | 14 Days |
| Total Projects | 2 |
| Developer | Yash Bisht |

## 📂 Project Overview

This repository serves as the central submission repository for both projects assigned during the Full-Stack Development internship.

Each project is maintained in its own independent GitHub repository and connected here using Git submodules. This preserves the individual project structures, source code, and commit histories.

| Project ID | Project Name | Category |
|---|---|---|
| FS-02 | NexaSync | Real-Time Collaborative Workspace |
| FS-03 | EduNexa | Learning Management System with Live Classes |

---

# FS-02 – NexaSync

## Real-Time Collaborative Workspace

<p align="center">
  <a href="https://collabespace-orcin.vercel.app/app">
    <img src="https://img.shields.io/badge/Live%20Demo-Visit%20Application-blue?style=for-the-badge" alt="NexaSync Live Demo" />
  </a>
  <a href="https://github.com/yash-bisht711/nexasync">
    <img src="https://img.shields.io/badge/GitHub-Source%20Code-black?style=for-the-badge&logo=github" alt="NexaSync Source Code" />
  </a>
</p>

### 1. Project Description

NexaSync is a real-time collaborative workspace designed to allow multiple users to work together on shared documents and collaborative boards.

The platform focuses on synchronized editing, real-time presence, workspace management, and collaborative productivity.

Inspired by modern collaborative tools such as Notion and Figma, NexaSync aims to provide a shared environment where users can collaborate while maintaining synchronized changes.

### 2. Key Features

- User authentication and workspace management.
- Collaborative pages and document editing.
- Rich-text editing using TipTap.
- Real-time synchronization using Yjs and WebSockets.
- Online user presence and collaboration indicators.
- Collaborative board functionality.
- Comments and discussions.
- Version history and document snapshots.
- Snapshot restoration.
- Workspace membership and access permissions.
- Redis-based infrastructure for synchronization across server instances.

### 3. Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | Next.js, React, TypeScript |
| Styling | Tailwind CSS |
| Editor | TipTap |
| Real-Time Collaboration | Yjs, WebSockets |
| Backend | Next.js server-side functionality and WebSocket server |
| Database | PostgreSQL |
| ORM | Prisma |
| Caching / Scaling | Redis |
| Validation | Zod |
| Deployment | Vercel and supporting backend infrastructure |

### 4. Architecture Overview

The application follows a full-stack architecture consisting of:

1. **Frontend Layer:** Provides the workspace interface, editor, collaborative boards, and user interactions.
2. **Authentication Layer:** Handles user identity and access to workspaces.
3. **Application Layer:** Manages workspaces, pages, comments, permissions, and snapshots.
4. **Collaboration Layer:** Uses Yjs and WebSockets to synchronize concurrent editing sessions.
5. **Data Layer:** PostgreSQL stores persistent application data through Prisma.
6. **Synchronization Infrastructure:** Redis supports communication and coordination across collaboration server instances.

### 5. Repository

- **Source Code:** https://github.com/yash-bisht711/nexasync
- **Live Application:** https://collabespace-orcin.vercel.app/app

---

# FS-03 – EduNexa

## Learning Management System with Live Classes

<p align="center">
  <a href="https://edu-nexa-iota.vercel.app/">
    <img src="https://img.shields.io/badge/Live%20Demo-Visit%20Application-blue?style=for-the-badge" alt="EduNexa Live Demo" />
  </a>
  <a href="https://github.com/yash-bisht711/EduNexa">
    <img src="https://img.shields.io/badge/GitHub-Source%20Code-black?style=for-the-badge&logo=github" alt="EduNexa Source Code" />
  </a>
</p>

### 1. Project Description

EduNexa is a full-stack Learning Management System designed to provide an integrated online learning environment for students, instructors, and administrators.

The platform brings together course management, video-based learning, live classes, assessments, certificates, and instructor earnings into one application.

Its objective is to simplify online education by connecting learning content, interactive sessions, and course administration.

### 2. Key Features

- Role-based access for students, instructors, and administrators.
- User authentication and profile management.
- Course creation and course enrollment.
- Video lesson management and uploading.
- Background video processing using FFmpeg and BullMQ.
- Video delivery infrastructure with CloudFront integration support.
- Live classes and real-time communication.
- Interactive quizzes and automatic grading.
- Student learning progress tracking.
- PDF certificate generation.
- Instructor revenue dashboard.
- Payment integration with test-mode support.
- Administrative course and platform management.

### 3. Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React, JavaScript |
| Styling | Tailwind CSS |
| State Management | Redux Toolkit |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| ODM | Mongoose |
| Background Jobs | BullMQ |
| Video Processing | FFmpeg |
| Real-Time Communication | Socket.IO, LiveKit |
| Storage | Cloudinary and video storage adapters |
| Payments | Razorpay test integration |
| Deployment | Vercel and Render |

**Database implementation note:** The current EduNexa implementation uses MongoDB and Mongoose.

### 4. Architecture Overview

The platform follows a modular full-stack architecture:

1. **Frontend Layer:** React-based interface for students, instructors, and administrators.
2. **API Layer:** Express.js REST APIs manage authentication, courses, enrollments, assessments, and payments.
3. **Authentication and Authorization:** Role-based access controls protect application resources.
4. **Database Layer:** MongoDB stores user, course, lesson, enrollment, and platform data.
5. **Media Processing Layer:** BullMQ workers process uploaded videos using FFmpeg.
6. **Real-Time Layer:** Socket.IO and LiveKit support interactive communication and live learning experiences.
7. **Payment Layer:** Payment workflows support test-mode integration.
8. **Deployment Layer:** Vercel hosts the frontend, while Render hosts the backend services.

### 5. Repository

- **Source Code:** https://github.com/yash-bisht711/EduNexa
- **Live Application:** https://edu-nexa-iota.vercel.app/
- **Backend:** https://edunexa-yzfg.onrender.com

---

# 🏗️ Overall Repository Structure

```text
Final-Internship-Submission/
│
├── README.md
├── .gitmodules
│
├── FS-02/                 # NexaSync Git Submodule
│   └── Original repository
│
└── FS-03/                 # EduNexa Git Submodule
    └── Original repository
```

Both projects retain their independent Git histories and development workflows.

---

# ⚙️ Getting Started

## Prerequisites

- Git
- Node.js and npm
- PostgreSQL (for NexaSync)
- MongoDB (for EduNexa)
- Redis (where required by the respective project)
- Visual Studio Code (recommended)

Additional environment variables and services may be required depending on each project's configuration.

## 1. Clone the Main Repository

Use the recursive clone command to download the parent repository and both project submodules.

```bash
git clone --recurse-submodules https://github.com/yash-bisht711/Final-Internship-Submission.git

cd Final-Internship-Submission
```

## 2. Initialize Submodules

If the repository was cloned without submodules, run:

```bash
git submodule update --init --recursive
```

## 3. Run NexaSync

Navigate to the NexaSync project:

```bash
cd FS-02
```

Follow the project-specific README for installation, environment configuration, database setup, and development commands.

Repository: https://github.com/yash-bisht711/nexasync

## 4. Run EduNexa

Navigate to the EduNexa project:

```bash
cd ../FS-03
```

Follow its project-specific README for installation, environment configuration, database setup, background workers, and development commands.

Repository: https://github.com/yash-bisht711/EduNexa

---

# 🧪 Testing and Quality Assurance

Testing and verification are important parts of both projects.

The individual project repositories contain their respective testing configurations and documentation.

The evaluation process should cover:

- Application startup and deployment verification.
- Authentication and authorization.
- Core application functionality.
- Database operations.
- API request and response validation.
- Real-time collaboration and communication.
- Error handling and edge cases.
- Role-based access restrictions.
- Cross-browser functionality where applicable.

Test results and performance measurements should be documented based on actual test execution.

---

# 📖 Project Documentation

Detailed technical documentation is maintained in the respective project repositories.

This includes:

- Project-specific README files.
- Installation and environment configuration.
- System architecture.
- Database design.
- API documentation.
- Testing instructions and results.
- Feature descriptions.

Additional presentation materials, architecture diagrams, screenshots, and individual reflections can be maintained in the `docs/` directory of this repository.

---

# 🚀 Live Deployments

| Project | Live Application | Source Code |
|---|---|---|
| NexaSync | [Open Application](https://collabespace-orcin.vercel.app/app) | [GitHub](https://github.com/yash-bisht711/nexasync) |
| EduNexa | [Open Application](https://edu-nexa-iota.vercel.app/) | [GitHub](https://github.com/yash-bisht711/EduNexa) |

---

# 🎯 Learning Outcomes

Through these projects, the development work focuses on practical full-stack engineering concepts, including:

- Designing and developing full-stack applications.
- Building REST APIs and managing databases.
- Authentication and role-based authorization.
- Real-time communication and collaborative systems.
- Background processing and media management.
- Integrating third-party services.
- Deploying and maintaining web applications.
- Writing maintainable code and technical documentation.
- Understanding application architecture and scalability.

---

# 👨‍💻 Developer

**Yash Bisht**

Full-Stack Developer

- **GitHub:** [yash-bisht711](https://github.com/yash-bisht711)
- **Portfolio:** [Personal Portfolio](https://yash-bisht711.github.io/Yash-Bisht_Portfolio/)

---

# 📜 Submission Information

This repository is prepared as the central GitHub submission for the Full-Stack Development internship.

It contains references to both assigned projects:

- **FS-02:** NexaSync – Real-Time Collaborative Workspace.
- **FS-03:** EduNexa – Learning Management System with Live Classes.

Both projects have their own public GitHub repositories and deployed application URLs.

**Thank you for reviewing this submission.**

<p align="center">
  <b>Built with dedication, continuous learning, and full-stack engineering.</b>
</p>