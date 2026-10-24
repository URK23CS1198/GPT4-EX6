# 🏥 MedAssist - AI-Powered Medical Symptom Assistant

## Experiment 6 - Building Applications using GPT-4
## URK23CS1198

An AI-powered clinical symptom evaluation assistant built using **Python, Flask, Ollama, and Llama 3.2**.

MedAssist assists users in understanding health symptoms, identifying potential medical conditions, highlighting missing clinical details, formulating intelligent follow-up questions, and providing medical attention guidance with integrated safety checks.

---

## 👤 Author
- **Name:** Madhavan S
- **Register Number:** URK23CS1198
- **Course:** Building Applications using GPT-4
- **Experiment:** 6 - AI-Powered Medical Symptom Assistant
- **Repository:** https://github.com/URK23CS1198/GPT4-EX6

---

## 🎯 Objective

To build an AI-Powered Medical Symptom Assistant that leverages local Large Language Models (Llama 3.2 via Ollama) and modular clinical workflows to structure patient inputs, evaluate symptoms, generate diagnostic hypotheses, provide safety recommendations, and support both CLI and Web interfaces.

---

## 🛠️ Technologies Used

- **Python**
- **Flask**
- **Ollama**
- **Llama 3.2**
- **HTML5 & CSS3**

---

## ✨ Features

- 👤 **Patient Profile Management:** Collects age, sex, duration, severity, past medical history, current medications, and known allergies.
- 🩺 **Intelligent Symptom Extraction:** Uses LLM prompting to parse natural-language complaints into structured clinical symptoms.
- 🔍 **Context Gap Detection:** Identifies critical missing information needed for assessment (e.g., onset timeline, specific triggers).
- 🧠 **AI Symptom Analysis:** Evaluates potential underlying causes and offers educational explanations.
- ❓ **Follow-Up Inquiry Generation:** Suggests specific clarifying questions to gather comprehensive clinical context.
- 🚨 **Safety & Red-Flag Guidance:** Identifies emergency warning signs requiring immediate healthcare attention.
- 📄 **Exportable Clinical Reports:** Automatically saves structured medical analysis reports (`outputs/medical_analysis.txt`).
- 🌐 **Web Dashboard & CLI:** Responsive healthcare interface with error handling and real-time processing, plus a full interactive terminal menu.

---

## 🔄 System Architecture & Workflow

```text
User / Patient Input (Symptoms, Vitals, History)
                       |
                       v
            Symptom Extraction Module
                       |
                       v
         Context & Missing Info Detection
                       |
                       v
           Medical Prompt Construction
                       |
                       v
             Ollama (Llama 3.2 LLM)
                       |
        +--------------+--------------+
        |                             |
        v                             v
Possible Conditions           Follow-Up Questions
        |                             |
        +--------------+--------------+
                       |
                       v
           Safety & Medical Guidance
                       |
        +--------------+--------------+
        |                             |
        v                             v
  Web Portal View             Exportable Report
```

---

## 📁 Project Structure

```text
GPT4-EX6/
├── data/
│   └── sample_cases.csv
├── outputs/
│   └── medical_analysis.txt
├── static/
│   └── style.css
├── templates/
│   └── index.html
├── analysis_module.py
├── app.py
├── context_module.py
├── input_module.py
├── main.py
├── profile_module.py
├── prompt_module.py
├── question_module.py
├── safety_module.py
├── save_module.py
├── symptom_module.py
├── test_symptoms.py
├── utils.py
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 🚀 Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/URK23CS1198/GPT4-EX6.git
cd GPT4-EX6
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Ensure Ollama is running with Llama 3.2
```bash
ollama run llama3.2
```

### 4. Run the Application

#### Option A: Web Interface (Flask)
```bash
python app.py
```
Open `http://127.0.0.1:5000` in your web browser.

#### Option B: Terminal / CLI Interface
```bash
python main.py
```

---

## ⚠️ Disclaimer

This application is an educational and informational tool powered by artificial intelligence. It does not provide medical diagnoses, treatment plans, or prescriptions, and is not a substitute for professional clinical judgment. Always seek immediate emergency medical care for acute or life-threatening symptoms.
