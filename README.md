# 🧠 Resume-JD Matcher App

This Streamlit application uses a multi-agent CrewAI architecture to intelligently match a candidate's resume with a job description (JD). The app also provides AI-generated resume enhancement suggestions and a tailored cover letter based on the uploaded content.

---

## 🚀 Features

- **Match Resume with Job Description**: Get a match score and reasoning.
- **Enhance Resume**: AI-powered suggestions to improve your resume for a given JD.
- **Generate Cover Letter**: Auto-generate a job-specific cover letter.
- **Visual Workflow**: Agent dependency graph displayed via Graphviz.

---


## 📁 Project Structure
```

├── ResumeJDMatchApp.py
├── CrewaiAgents/
│ ├── ResumeParsingAgent.py
│ ├── JDUnderstandingAgent.py
│ ├── MatchingAgent.py
│ ├── ResumeEnhancerAgent.py
│ └── CoverLetterAgent.py
├── requirements.txt
├── .env
└── README.md
```

---

## ⚙️ Prerequisites

### 1. Python Version

Ensure you're using Python 3.8 or above.

### 2. Environment Setup

Clone the repo:

```
git clone https://github.com/vikrambhat2/MultiAgents-with-CrewAI-ResumeJDMatcher.git
cd MultiAgents-with-CrewAI-ResumeJDMatcher
```
Create and activate a virtual environment:

```
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```
Install dependencies:
```
pip install -r requirements.txt
```
Make sure you have Graphviz installed for full graph visualization.

3. Environment Variables
Create a .env file in the root directory if needed (can be left empty if using only local models).

🧠 Local Model Setup
This app expects a local Ollama instance running llama3.2.

#### Install Ollama
Follow instructions at https://ollama.com.

#### Run the LLaMA 3.2 Model
```
ollama run llama3:instruct
```
### ▶️ Running the App
Start the Streamlit app:

```
streamlit run ResumeJDMatchApp.py
```

###  🖥️ How to Use
Upload or paste your resume and job description.

Choose an action:
-  🚀 Run Matching — to evaluate alignment.
-  📝 Enhance Resume — to get resume improvement tips.
- ✉️ Generate Cover Letter — to generate a personalized cover letter.

Results will be displayed below the buttons.

### 📦 Outputs
- ✅ Match Report
- 🔧 Resume Enhancement Suggestions
- 💌 Generated Cover Letter

### 🙌 Acknowledgments
Built using CrewAI, Streamlit, and Ollama.
