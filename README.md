# 🚀 FreelanceFlow

A modern full-stack freelancing ecosystem that connects **Clients**, **Freelancers**, and **Learners** through a unified platform for project discovery, internships, collaboration, and skill development.

FreelanceFlow combines:

- 💼 Freelance Project Marketplace
- 🎯 Internship Discovery Portal
- 💬 Communication System
- 🎓 Learning & Upskilling Hub
- 🤖 AI-Powered Document Processing
- 🔐 Secure Role-Based Authentication

---

## 📌 Overview

FreelanceFlow is a MERN-stack based platform designed to bridge the gap between clients and freelancers while also supporting continuous learning and career growth. The platform enables users to discover freelance opportunities, internships, and curated learning resources in one place.

---

## ✨ Features

### 🔐 Authentication & Authorization

- JWT-based Authentication
- Secure Password Hashing using Bcrypt
- Role-Based Access Control (RBAC)

#### User Roles

**Client**
- Post Projects
- Manage Applications
- Hire Freelancers

**Freelancer**
- Browse Projects
- Apply for Opportunities
- Explore Learning Resources

**Admin**
- Manage Users
- Monitor Platform Activities
- Manage Learning Content

---

### 💼 Freelance Marketplace

- Create and manage projects
- Browse available opportunities
- Submit project proposals
- Search and filter projects
- Skill-based opportunity discovery

---

### 🎯 Internship Portal

- Dedicated internship listings
- Beginner-friendly opportunities
- Category-based filtering
- Career development support

---

### 🎓 Learning & Upskilling Hub

- Curated course recommendations
- Domain-based filtering
- Difficulty-level categorization
- Provider-based search
- Learning resource discovery

#### Supported Learning Providers

- Coursera
- Google
- Udemy
- edX
- LinkedIn Learning

---

### 💬 Communication System

- Direct client-freelancer interaction
- Project discussions
- Collaboration support

---

### 🤖 AI-Powered Document Processing

Clients can upload requirement documents for analysis.

#### Supported Formats

- PDF
- DOCX

#### Features

- Text Extraction
- Requirement Parsing
- Skill Identification
- Content Analysis

---

## 🏗️ System Architecture

```text
Frontend (React + Tailwind CSS)
            │
            ▼
Backend (Node.js + Express)
            │
 ┌──────────┼──────────┐
 ▼          ▼          ▼
MongoDB   JSON Store  NLP Service
                        │
                        ▼
                 Flask + spaCy
```

---

## 🛠️ Technology Stack

### Frontend

- React.js
- Vite
- Tailwind CSS
- React Router DOM
- Lucide React

### Backend

- Node.js
- Express.js
- JWT
- Bcrypt.js
- Multer
- CORS

### Database

- MongoDB
- Mongoose

### AI & NLP

- Python
- Flask
- spaCy
- TextBlob

### Document Processing

- pdf-parse
- mammoth

---

## 📂 Project Structure

```text
FreelanceFlow/
│
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── data/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── app.js
│   │   └── server.js
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── main.jsx
│
├── package.json
└── README.md
```

---

## ⚙️ Installation

### Prerequisites

- Node.js (v18 or higher)
- npm (v9 or higher)
- MongoDB

### Clone Repository

```bash
git clone https://github.com/your-username/FreelanceFlow.git
cd FreelanceFlow
```

### Install Dependencies

```bash
npm install
npm run install:all
```

### Configure Environment Variables

Create a `.env` file inside the backend folder.

```env
PORT=5000
JWT_SECRET=your_secret_key
MONGO_URI=mongodb://localhost:27017/freelanceflow
```

### Run the Application

```bash
npm run dev
```

Frontend:

```text
http://localhost:5173
```

Backend:

```text
http://localhost:5000
```

---

## 📡 API Endpoints

| Endpoint | Method | Description |
|-----------|---------|-------------|
| /api/auth/register | POST | Register User |
| /api/auth/login | POST | User Login |
| /api/projects | GET | Fetch Projects |
| /api/projects | POST | Create Project |
| /api/applications | POST | Submit Proposal |
| /api/courses | GET | Fetch Learning Courses |
| /api/learning-posts | GET | Learning Resources |
| /api/admin/dashboard | GET | Admin Dashboard |

---

## 🚀 Future Enhancements

- Real-Time Chat using WebSockets
- AI-Based Project Recommendation
- Freelancer Rating System
- Resume Analysis System
- Payment Gateway Integration
- Mobile Application
- Advanced Learning Analytics

---

## 👩‍💻 Developer

**K. Tejasree**

Full Stack Developer | MERN Stack | AI/ML Enthusiast

---

## 📄 License

This project is developed for educational and portfolio purposes.
Feel free to fork, learn from, and build upon it.
