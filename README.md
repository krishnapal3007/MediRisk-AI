# 🫀 MediRisk AI — Heart Disease Risk Prediction

MediRisk AI is a machine learning-powered web application that estimates the risk of heart disease based on clinical and lifestyle-related health parameters.

The application provides an easy-to-use health assessment dashboard, AI-powered health assistance, risk analysis, health insights, and downloadable PDF reports.

> ⚠️ **Educational Disclaimer:** MediRisk AI is an educational project and is not a medical diagnosis or a substitute for professional medical advice.

---

## 🚀 Live Demo

🌐 **Live Website:**  
https://medirisk-ai-calh.onrender.com/

📂 **GitHub Repository:**  
https://github.com/krishnapal3007/MediRisk-AI

---

## ✨ Features

- 🫀 Heart disease risk prediction
- 🤖 Machine Learning-based analysis
- 📊 Risk probability and risk level
- 🧮 Automatic BMI calculation
- 🩺 Clinical health assessment
- 🧑‍⚕️ Lifestyle risk assessment
- 💬 AI Health Assistant
- 📄 Downloadable PDF health report
- 📈 Health score and personalized insights
- 🔄 What-if risk simulation
- 📱 Responsive desktop and mobile interface
- 🔐 Environment variable support for API keys

---

## 🧠 Machine Learning

MediRisk AI uses multiple machine learning algorithms during model evaluation:

- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

### 🏆 Best Model

**Random Forest**

| Metric | Score |
|---|---:|
| Accuracy | 86.67% |
| Precision | 88.46% |
| Recall | 82.14% |
| F1 Score | 85.19% |
| ROC-AUC | 94.20% |

The final application uses the trained Random Forest model for prediction.

---

## 📊 Dataset

The project uses the **UCI Cleveland Heart Disease dataset**.

### Dataset Information

- Original records: **303**
- Features: **13 clinical features**
- Target: Heart disease presence/absence
- Missing values handled during preprocessing
- Target converted into a binary classification problem

### Clinical Features

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Maximum Heart Rate
- Exercise-Induced Angina
- Oldpeak
- Slope
- Major Vessels
- Thalassemia

---

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript
- Font Awesome
- Google Fonts

### Backend
- Python
- Flask

### Machine Learning
- Scikit-learn
- Pandas
- NumPy
- Joblib

### AI
- OpenAI API

### Reporting
- ReportLab

### Deployment
- Render
- Gunicorn

---

## 📁 Project Structure

```text
MediRisk_AI/
│
├── app.py
├── train.py
├── predict.py
├── best_model.pkl
├── scaler.pkl
├── requirements.txt
├── README.md
├── .gitignore
│
├── dataset/
│   └── heart.csv
│
├── templates/
│   ├── home.html
│   └── index.html
│
└── static/
    ├── style.css
    └── professional.css
