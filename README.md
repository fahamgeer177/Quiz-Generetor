# 🎯 Quiz Generator Project

Create quizzes from documents using AI, evaluate generated content quality, and experiment with question generation datasets in one workspace.

## ✨ Highlights

- 📄 Upload PDF, DOCX, or PPTX files and extract text
- 🤖 Generate quiz questions and answers with OpenAI
- 📊 Evaluate generated content using BLEU, METEOR, and ROUGE metrics
- 🧪 Includes dataset conversion and experimentation scripts
- 🖥️ Streamlit-based interface for quick local usage

## 🧱 Main Files

- `app.py` : Document-to-quiz Streamlit app
- `eval.py` : Document-to-quiz app with quality evaluation metrics
- `conv.py` : Converts SQuAD v2 JSON into CSV format
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

### Document to Quiz Generator + Evaluation

```bash
streamlit run eval.py
```

### Convert SQuAD v2 to CSV

```bash
python conv.py
```

## 📈 Evaluation Metrics Used

- BLEU
- METEOR
- ROUGE-1
- ROUGE-2
- ROUGE-L

## 🛡️ GitHub Push Readiness Checklist

- ✅ Dependencies documented in `requirements.txt`
- ✅ README added with setup and usage instructions
- ✅ API key moved to environment variable (`OPENAI_API_KEY`)
- ✅ Root `.gitignore` added (venv, secrets, caches, node_modules, and large local artifacts)
- ⚠️ If the old API key was real, rotate it immediately in your OpenAI dashboard

## 📤 Push To GitHub

Use these commands from the project root after creating an empty GitHub repository:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## 🗂️ Notes

This workspace also contains additional datasets and sub-projects (for example `RACE/`, `LearningQ-qg/`, `SQuAD-explorer/`, and `my-next-app/`) that can support future improvements and experiments.

---

Built for learning, experimentation, and rapid prototyping of AI-powered quiz generation. 🚀
