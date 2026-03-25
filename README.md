# 🎯 Quiz Generator Project

Create quizzes from documents using AI, evaluate generated content quality, and experiment with question generation datasets in one workspace.

https://github.com/user-attachments/assets/3fa6bf56-8483-4fa7-8f51-b66304e48521

## ✨ Highlights

- 📄 Upload PDF, DOCX, or PPTX files and extract text
- 🤖 Generate quiz questions and answers with OpenAI
- 🖥️ Streamlit-based interface for quick local usage

## 🧱 Main Files

- `app.py` : Document-to-quiz Streamlit app
- `requirements.txt` : Python dependencies for the project

## ⚙️ Setup

### 1) Create and activate a virtual environment

#### Windows (PowerShell)

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

#### macOS/Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2) Install dependencies

```bash
pip install -r requirements.txt
```

### 3) Configure environment variables

Set your OpenAI key in an environment variable (do not hardcode secrets in files):

You can also copy values from `.env.example` into your local environment.

#### Windows (PowerShell)

```powershell
$env:OPENAI_API_KEY="your_openai_api_key_here"
```

#### macOS/Linux

```bash
export OPENAI_API_KEY="your_openai_api_key_here"
```

## 🚀 Run The Apps

### Document to Quiz Generator

```bash
streamlit run app.py
```

 ## Licence

 MIT
---

Built for learning, experimentation, and rapid prototyping of AI-powered quiz generation. 🚀
