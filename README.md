# Automated Resume Relevance Check System
AI-powered Automated Resume Relevance Check System for evaluating resumes against job descriptions with hybrid scoring, semantic analysis, and a web dashboard.

## 🔍 What is this?

This system automates resume evaluation so placement teams can select students faster and more consistently. Students upload resumes, placement teams upload or select job descriptions, and the system scores each resume per JD — giving a final relevance score, missing skills, and personalized feedback.

## 🌐 Live Demo

Try the deployed Streamlit app here:  
[Automated Resume Relevance Check System](https://sakshiphand-automated-resume-relevance-checker-app-366big.streamlit.app/)

## 🎬 Demo Video

Check out the full demo on YouTube:  
[Watch on YouTube](https://youtu.be/ET8otLacdSM?si=S5hdJoZrQQ9Vc18p)

## ✅ Features

| Feature                                   | Description                                                                 |
|-------------------------------------------|-----------------------------------------------------------------------------|
| 📂 Resume Upload                          | Accepts resumes in **PDF/DOCX** format uploaded at runtime                  |
| 📄 Job Description Upload                 | Placement team uploads/selects JD files from the `jd/` folder               |
| 🔍 Resume Parsing                         | Extracts raw text, normalizes sections, removes headers/footers             |
| 📝 JD Parsing                             | Extracts role title, must-have skills, good-to-have skills, qualifications  |
| ⚡ Hard Match                             | Keyword/skill/education matching (exact + fuzzy matches)                    |
| 🤖 Semantic Match                         | Embedding-based similarity + optional LLM reasoning                         |
| 📊 Hybrid Scoring                         | Combines hard + semantic match with weighted scoring formula                |
| 📈 Output Generation                      | Generates Relevance Score (0-100), Missing Skills, Verdict (High/Med/Low)   |
| 💡 Suggestions                           | Provides improvement tips for missing skills, certifications, projects      |
| 🗄️ Storage & Database                    | Stores results in **SQLite** for future access                              |
| 🔎 Dashboard Filtering                    | Placement team can filter/search by job role, score, location, verdict      |
| 🌐 Web Application                        | Streamlit dashboard for uploading JDs/resumes and viewing results           |
| 📥 Export Results                         | Download CSV reports for each JD separately                                 |

## Result

![WhatsApp Image 2025-09-21 at 1 55 26 PM](https://github.com/user-attachments/assets/89e17ca2-7337-4f20-ba78-e875694fa0d5)

![WhatsApp Image 2025-09-21 at 1 55 27 PM](https://github.com/user-attachments/assets/b26106aa-9deb-4694-ac55-fc94086f1381)

## 🚀 Getting Started

Follow these steps to set up and run the Automated Resume Relevance Check System on your local machine.

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/YourUsername/Automated-Resume-Relevance-Check.git
cd Automated-Resume-Relevance-Check
```
2️⃣ Create a Virtual Environment (Recommended)
```bash
python -m venv venv
```
Activate it depending on your OS:
#### Windows:
```bash
venv\Scripts\activate
```
#### Mac/Linux:
```bash
source venv/bin/activate
```
### 3️⃣ Install Dependencies
#### Install all required packages:
```bash
pip install -r requirements.txt
```
#### Additionally, download the SpaCy English language model:
```bash
python -m spacy download en_core_web_sm
```
### 4️⃣ Run the Application
#### Launch the Streamlit web application with:
```bash
streamlit run app.py
```

## Usage
1. Upload one or more Job Descriptions (JD) in PDF/DOCX format.
2. Upload student Resumes in PDF/DOCX format.
3. The system will automatically:
       Parse text from resumes and JDs
       Perform hard + semantic matching
       Generate a Relevance Score (0–100), Missing Skills, and Verdict
5. View results in the Streamlit dashboard with filtering/search options.
6. Export results as CSV reports for the placement team.









