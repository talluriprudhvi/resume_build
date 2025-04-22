# 🧠 AI Resume Generator (Flask + OpenAI + DOCX)

This project is a simple Flask-based backend service that generates **ATS-optimized resumes** using OpenAI's GPT models. It accepts personal and professional input via API, generates a professional resume with detailed summaries and experience, and returns it as a downloadable `.docx` file.

---

## ✨ Features

- Generate AI-written **Professional Summaries** (10+ lines minimum)
- Write detailed **Experience sections** (10+ lines per job role)
- Automatically formats the resume with bold section headers
- Excludes placeholder fields like `[Name]`, `[Email]`, etc.
- Returns a downloadable Word document
- Cross-origin support via CORS

---

## 🛠️ Technologies Used

- Python 3
- Flask
- OpenAI API (GPT-4o)
- `python-docx` for generating Word documents
- `flask-cors` for frontend-backend communication

---

## 📦 Installation

1. **Clone the repository**

```bash
git clone https://github.com/talluriprudhvi/resume_build.git
cd ai-resume-generator


✅ Sample Request
curl -X POST http://127.0.0.1:5000/generate_resume \
     -H "Content-Type: application/json" \
     -d '{
           "name": "NAME",
           "title": "Senior AI/ML Engineer",
           "in_message": "Senior AI Engineer with 9 years of experience specializing in generative AI worked in capgemini from 2020 to 2024 and now I am working at Lava Data with B.Tech from JNTUH. I am AWS certified."
         }' --output resume.docx