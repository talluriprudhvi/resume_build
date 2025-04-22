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
git clone https://github.com/yourusername/ai-resume-generator.git
cd ai-resume-generator