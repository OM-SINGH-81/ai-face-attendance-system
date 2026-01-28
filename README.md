# AI-Based Face Recognition Attendance System

An intelligent, real-time attendance management system that automates student attendance using **AI-powered face recognition** with **liveness verification** to prevent proxy attendance.

---

## 🚀 Project Overview

Traditional attendance systems are:
- Time-consuming
- Error-prone
- Easily manipulated through proxies

This project solves these issues by using **real-time face recognition with live camera feeds**, ensuring **accurate, secure, and automated attendance tracking**.

The system is designed to be managed by **teachers or administrators** and supports **multiple cameras**, making it scalable for classrooms, labs, and institutions.

---

## 🎯 Key Features

- ✅ **Real-time face recognition**
- ✅ **Automatic check-in and check-out**
- ✅ **Daily attendance reset (new day, new record)**
- ✅ **Anti-proxy protection using liveness detection (eye blink)**
- ✅ **Multi-camera support**
- ✅ **Admin-controlled student authorization**
- ✅ **Searchable attendance logs (date-wise & student-wise)**
- ✅ **Secure authentication system**
- ✅ **Scalable architecture for future expansion**

---

## 🧠 System Workflow

1. **Student Registration**
   - Student submits details and facial image
   - Admin authorizes the student

2. **Live Attendance**
   - Camera captures live video feed
   - Face detected using **MTCNN**
   - Facial embeddings generated using **FaceNet**
   - Identity matched with registered students

3. **Liveness Verification**
   - Eye-blink detection ensures the person is live
   - Prevents photo/video-based proxy attendance

4. **Attendance Logging**
   - Automatic check-in on first recognition
   - Automatic check-out after a fixed time interval
   - Attendance stored with timestamps in database

---

## 🛠️ Technology Stack

### Backend
- **Python**
- **Django**

### AI / Computer Vision
- **FaceNet** (Face embeddings)
- **MTCNN** (Face detection)
- **MediaPipe** (Eye-blink liveness detection)
- **OpenCV**

### Database
- **SQLite** (can be replaced with PostgreSQL/MySQL)

### Frontend
- **HTML**
- **CSS**
- **Bootstrap**

### Security
- **Django Authentication System**
- Role-based access (Admin / User)

---

## 📂 Project Structure

Project101/
│
├── app1/
│ ├── models.py
│ ├── views.py
│ ├── urls.py
│ └── templates/
│
├── Project101/
│ ├── settings.py
│ ├── urls.py
│
├── media/
├── static/
├── manage.py
└── README.md

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository
```bash
git clone https://github.com/OM-INGH-81/ai-face-attendance-system.git
cd ai-face-attendance-system
