# 🚀 Resume Analyzer Based on Job Description

This project is a **Resume Analyzer Web App** that evaluates how well a resume matches a given job description (JD). It uses OCR to extract text from PDF/image resumes, compares keywords against predefined job role skills, calculates an **ATS (Applicant Tracking System) score**, and recommends the most suitable job roles.

## 🔍 Features

- 📄 **PDF/Image Resume Support** – Uses OCR (Tesseract + pdf2image) to extract text from resumes.
- 🧠 **Role-Based Skill Matching** – Compares resume skills with predefined skill sets for roles like:
  - AI/ML Intern
  - Data Analyst
  - Web Developer
  - Backend Developer
  - Cloud Engineer
  - DevOps Engineer
  - Cybersecurity Analyst
  - Data Scientist
  - Business Analyst
  - Full Stack Developer
- 📊 **ATS Score Visualization** – Generates a pie chart showing match vs. missing skills.
- 💬 **Smart Suggestions** – Gives actionable feedback and best-fit job roles based on skill matching.
- ⚙️ **Gradio Interface** – Intuitive UI to upload resumes and paste job descriptions.

## 🛠️ Tech Stack

- **Python**
- **Gradio** – for the interactive web interface
- **PyMuPDF (fitz)** – for PDF reading
- **pdf2image** – for converting PDF to image
- **pytesseract** – for OCR text extraction
- **NLTK** – for text processing and keyword extraction
- **Matplotlib** – for generating the ATS pie chart

## 📦 Installation

First, install the required dependencies:

```bash
pip install gradio pdf2image pytesseract nltk matplotlib PyMuPDF
sudo apt-get install -y poppler-utils
```

Also, make sure Tesseract OCR is installed and accessible in your environment.

## ▶️ How to Use

1. Run the script:

```bash
python resume_checker.py
```

2. A Gradio interface will open in your browser.
3. Upload your resume (PDF or image).
4. Paste the job description.
5. View your ATS score, pie chart, and suggestions for improvement.

## 📸 Sample Output

*(You can add screenshots of the UI or ATS pie chart here)*

## 📄 License

This project is for educational and non-commercial use.

---

**Note:** The matching logic is based on static keyword lists and does not represent real-world ATS software. Always tailor your resume to each job manually.
