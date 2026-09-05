# AI Resume Analyzer

An end-to-end Python web application built with Streamlit and Natural Language Processing (NLP) to parse PDF resumes, extract candidate skillsets, score structural completeness, and provide domain-specific course recommendations.

---

## Key Features

- **Automated Resume Parsing:** Extracts contact info, educational history, work experience, and technical skill keywords using `pyresparser`, `spaCy`, and `NLTK`.
- **Structural Scoring & Feedback:** Evaluates critical sections (Objective, Experience, Education, Projects) and provides targeted improvement recommendations.
- **Smart Course Recommendations:** Predicts domain alignment (e.g., Web Development, Data Science, Android Dev, DevOps) and suggests relevant learning resources.
- **Dual Portal Support:**
  - **Candidate View:** Upload resume, review extracted skill profiles, view layout scores, and get learning paths.
  - **Admin View:** Review historical applicant data and submission analytics.
- **Clean File Hygiene:** Git-ignored upload management, clean folder architecture, and dynamic visitor metrics.

---

## Tech Stack

- **Frontend & App Framework:** [Streamlit](https://streamlit.io/)
- **Core Language:** Python 3.10+
- **NLP Engine:** `spaCy` (`en_core_web_sm`), `NLTK`, `pyresparser`, `pdfminer.six`
- **Data & Storage:** `pandas`, `pypdf`, SQLite
- **Version Control:** Git & GitHub

---

## Repository Structure

```text
AI-Resume-Analyzer/
├── App/
│   ├── App.py                  # Main Streamlit application entry point
│   ├── Courses.py              # Skill and course recommendation mappings
│   ├── requirements.txt        # Python library dependencies
│   └── Uploaded_Resumes/       # Directory for processing PDF files
├── pyresparser/
│   └── resume_parser.py        # Core extraction and parsing logic
├── .gitignore                  # Git tracking rules
├── LICENSE                     # MIT License
└── README.md                   # Project documentation