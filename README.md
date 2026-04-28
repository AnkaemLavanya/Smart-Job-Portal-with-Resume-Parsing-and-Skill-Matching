# Smart-Job-Portal-with-Resume-Parsing-and-Skill-Matching
This full-stack job portal connects recruiters and job seekers, enabling job posting, searching, and resume-based applications. It uses PyPDF2 for resume parsing and rule-based skill matching to generate scores, with JWT authentication and role-based access for secure and scalable use.
# 💼 Smart Job Portal

A full-stack web application that connects **job seekers** and **recruiters** on a single platform.  
Recruiters can post and manage jobs, while job seekers can search, apply, and analyze their resumes.

---

## 🚀 Features

### 👨‍💼 Recruiter
- Post new jobs
- Edit job details
- Delete job postings
- View number of applicants

### 👩‍💻 Job Seeker
- Search jobs with filters
- Apply with resume upload (PDF)
- View application results and match score

### 📄 Resume Analysis
- Extracts text from PDF resumes using PyPDF2
- Matches skills with job requirements
- Generates:
  - Match Score (%)
  - Matched Skills
  - Missing Skills

### 🔐 Authentication
- JWT-based authentication
- Role-based access (Recruiter / Job Seeker)

---

## 🛠️ Tech Stack

### Frontend
- React.js (Vite)
- React Router
- JavaScript (ES6)
- HTML, CSS

### Backend
- Django
- Django REST Framework (DRF)

### Database
- MySQL

### Libraries / Tools
- PyPDF2 (Resume parsing)
- Fetch API
- CORS Headers

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository
```bash
git clone https://github.com/your-username/job-portal.git
cd job-portal
2️⃣ Backend Setup (Django)
cd backend
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
3️⃣ Frontend Setup (React)
cd frontend
npm install
npm run dev
🔑 API Endpoints
Method	Endpoint	Description
GET	/api/jobs/	Get all jobs
POST	/api/login/	User login
POST	/api/signup/	User registration
POST	/api/apply/	Apply for job
GET	/api/dashboard/	Dashboard data
POST	/api/post-job/	Create job
PUT	/api/edit-job/:id/	Edit job
DELETE	/api/delete-job/:id/	Delete job
🧠 How It Works
User signs up as Job Seeker or Recruiter
Recruiter posts job with required skills
Job seeker uploads resume (PDF)
System extracts text using PyPDF2
Skills are matched using keyword comparison
Match score and analysis are generated
📌 Future Improvements
AI/ML-based resume analysis
Email notifications
Resume ranking system
Advanced filters & recommendations
