# 🫀 MediRisk AI

### AI-Powered Heart Disease Risk Assessment Platform

MediRisk AI is a machine learning-based web application that provides an **educational assessment of potential heart disease risk** using clinical health parameters.

The platform combines a trained **Random Forest classifier** with a Flask web application to provide risk probability, risk classification, health scoring, explainable insights, personalized recommendations, risk history, what-if simulation, PDF reporting, and an assessment-aware AI Health Assistant.

> ⚠️ **Medical Disclaimer:** MediRisk AI is an educational and demonstration project. It is not a medical diagnostic system and must not be used as a substitute for professional medical advice, diagnosis, or treatment.

---

## ✨ Features

- 🫀 Heart disease risk prediction
- 📊 Risk probability analysis
- 🎯 Low / Moderate / High risk classification
- 💯 Educational health score
- 📈 Explainable AI and top model factors
- 🔬 What-If risk simulator
- 📈 Assessment history and risk trend
- 💡 Personalized educational recommendations
- 📋 Assessment summary
- 🤖 Assessment-aware AI Health Assistant
- 💬 Interactive chat with quick prompts
- 🧹 Clear chat and conversation context
- 📄 Downloadable PDF assessment report
- 📱 Responsive healthcare dashboard
- 🔐 Environment-variable based API configuration

---

## 🧠 Machine Learning

The project evaluates multiple algorithms:

- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

### 🏆 Selected Model — Random Forest

| Metric | Score |
|---|---:|
| Accuracy | **86.67%** |
| Precision | **88.46%** |
| Recall | **82.14%** |
| F1 Score | **85.19%** |
| ROC-AUC | **94.20%** |

The trained model is stored in `best_model.pkl` and the preprocessing scaler is stored in `scaler.pkl`.

---

## 📊 Dataset

MediRisk AI uses the **UCI Heart Disease Dataset (Cleveland)**.

- Original records: **303**
- Records after removing missing values: **297**
- Input features: **13**
- Target: binary heart disease classification

### Input Features

`age` · `sex` · `cp` · `trestbps` · `chol` · `fbs` · `restecg` · `thalach` · `exang` · `oldpeak` · `slope` · `ca` · `thal`

---

## 🛠️ Technology Stack

**Frontend**
- HTML5
- CSS3
- JavaScript
- Font Awesome

**Backend**
- Python
- Flask

**Machine Learning**
- Scikit-learn
- XGBoost
- Pandas
- NumPy
- Joblib

**AI**
- OpenAI API

**Reporting**
- ReportLab

---

## 📁 Project Structure

```text
MediRisk_AI/
│
├── dataset/
│   └── heart.csv
│
├── static/
│   ├── style.css
│   └── professional.css
│
├── templates/
│   ├── home.html
│   └── index.html
│
├── app.py
├── train.py
├── predict.py
├── best_model.pkl
├── scaler.pkl
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/MediRisk-AI.git
cd MediRisk-AI
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the environment

**Windows**

```powershell
venv\Scripts\activate
```

**macOS / Linux**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔐 Environment Configuration

Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key_here
OPENAI_MODEL=your_openai_model_here
FLASK_SECRET_KEY=change-this-secret
```

Never commit `.env` to GitHub.

The repository includes `.env.example` as a safe template.

---

## ▶️ Run Locally

```bash
python app.py
```

Open:

```text
http://127.0.0.1:5000
```

A lightweight health endpoint is also available at:

```text
/health
```

---

## 🔍 Application Workflow

```text
Patient Health Assessment
          ↓
Input Validation & Preprocessing
          ↓
Feature Scaling
          ↓
Random Forest Classifier
          ↓
Risk Probability
          ↓
Risk Classification
          ↓
Health Score + Explainable Insights
          ↓
Recommendations + What-If Analysis
          ↓
AI Health Assistant
```

---

## 🤖 AI Health Assistant

The AI Health Assistant uses the current assessment context to help users understand their results.

Example questions:

- Why is my risk high?
- Explain my prediction.
- What are the key factors affecting my result?
- What does my cholesterol value mean?
- Give me practical next steps.
- What questions should I ask my doctor?

The assistant is designed for **educational health information only**. It does not diagnose conditions or prescribe treatment.

---

## 🔬 Explainable AI

MediRisk AI provides model-factor information alongside the prediction so users can better understand which clinical parameters were considered important by the trained model.

Feature importance should be interpreted as **model behavior**, not as proof that a particular factor caused an individual's medical outcome.

---

## 📈 What-If Simulator

The What-If Simulator allows users to change selected clinical parameters and observe how the trained model's predicted probability changes.

This feature is intended to demonstrate model behavior and should not be interpreted as a clinical intervention simulator.

---

## 📄 PDF Reporting

Users can generate a downloadable assessment report containing relevant patient inputs, prediction information, and educational insights.

Reports are generated using **ReportLab**.

---

## 🔒 Security

- API keys are loaded through environment variables.
- `.env` is excluded from version control.
- `venv/` is excluded from version control.
- Python cache files are excluded.
- Sensitive credentials are not hard-coded.

---

## ⚠️ Medical Disclaimer

This application is a **portfolio and educational Machine Learning project**.

A model prediction is a statistical estimate and **not a medical diagnosis**.

Do not use MediRisk AI to:

- Diagnose heart disease
- Start or stop medication
- Replace a qualified healthcare professional
- Make emergency medical decisions

For medical concerns, consult a qualified healthcare professional.

---

## 🚀 Future Improvements

- SHAP-based advanced explainability
- Model calibration
- Larger and more diverse datasets
- User authentication
- Secure database integration
- Cloud deployment
- Doctor consultation workflow
- Mobile application
- Real-time health data integration
- Model monitoring

---

## 👨‍💻 Author

**Krishna**

B.Tech — Artificial Intelligence & Machine Learning

**Interests:** Artificial Intelligence · Machine Learning · Python · Deep Learning · AI Applications

---

## ⭐ Project Status

**Active Development**

MediRisk AI is being continuously improved with new AI, explainability, visualization, and user-experience features.

---

## 📜 License

This project is intended for educational, research, and portfolio purposes.
