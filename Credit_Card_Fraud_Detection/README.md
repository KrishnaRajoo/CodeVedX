# 🛡️ AI Fraud Shield  
## Credit Card Fraud Detection System Using Machine Learning & Explainable AI

<p align="center">

<img src="static/images/favicon.png" width="120">

</p>

<p align="center">
An intelligent machine learning system that detects fraudulent credit card transactions using advanced classification algorithms and provides transparent AI explanations using SHAP.
</p>


---
Live Application: https://credit-card-fraud-detection-system-c8f4.onrender.com

# 🚀 Project Overview

Financial fraud is one of the biggest challenges in digital transactions. This project builds an AI-powered fraud detection system capable of identifying suspicious credit card transactions and classifying them as:

- ✅ Genuine Transaction
- 🚨 Fraudulent Transaction

The system uses machine learning techniques to handle highly imbalanced transaction data, train classification models, evaluate performance, and provide explainable predictions.

---

# ✨ Features

## 🔐 Fraud Detection

- Real-time transaction fraud prediction
- Fraud probability estimation
- Risk level classification
- Confidence score generation


## 🤖 Machine Learning Pipeline

- Data preprocessing
- Feature normalization
- Class imbalance handling
- Model comparison
- Performance evaluation


## 🧠 Explainable AI

Using SHAP (SHapley Additive exPlanations):

- Understand why a transaction was classified as fraud
- Feature importance visualization
- Transparent AI decision-making


## 🎨 Modern Web Interface

- Premium red-black cybersecurity theme
- Responsive design
- Mobile hamburger navigation
- Interactive prediction dashboard
- Animated UI components

---

# 🏗️ System Architecture


```
                 Transaction Data

                        |
                        ↓

              Data Preprocessing

                        |
                        ↓

             Class Imbalance Handling

                  (SMOTE)

                        |
                        ↓

              Machine Learning Models

       ┌────────────────────────────┐
       │ Logistic Regression        │
       │ Random Forest ⭐           │
       │ XGBoost                    │
       └────────────────────────────┘

                        |
                        ↓

             Best Model Selection

             Random Forest Classifier

                        |
                        ↓

              Fraud Prediction API

                        |
                        ↓

              Flask Web Application

                        |
                        ↓

              Explainable AI (SHAP)

```

---

# 📊 Dataset Information

Dataset:

**Credit Card Fraud Detection Dataset**

Source:

Kaggle Credit Card Fraud Dataset


## Dataset Statistics

| Information | Value |
|---|---:|
| Total Transactions | 284,807 |
| Fraud Transactions | 492 |
| Genuine Transactions | 284,315 |
| Features | 30 |
| Fraud Ratio | 0.172% |


The dataset contains:

- Time
- Amount
- PCA transformed features (V1-V28)
- Class label

Where:

```
0 → Genuine Transaction

1 → Fraudulent Transaction
```

---

# ⚙️ Machine Learning Workflow


## 1. Data Preprocessing

Performed:

- Missing value analysis
- Feature scaling
- Data normalization
- Train-test split


## 2. Handling Class Imbalance

Credit card fraud datasets are highly imbalanced.

Applied:

**SMOTE (Synthetic Minority Oversampling Technique)**

to improve fraud detection capability.


## 3. Model Training

Implemented models:

| Model | Purpose |
|---|---|
| Logistic Regression | Baseline model |
| Random Forest | Final selected model |
| XGBoost | Advanced comparison model |


---

# 🏆 Model Performance

## Final Model

### Random Forest Classifier


| Metric | Score |
|---|---:|
| Accuracy | 99.94% |
| Precision | 82.47% |
| Recall | 81.63% |
| F1 Score | 82.05% |
| ROC-AUC | 98.32% |


Random Forest was selected because it provided the best balance between:

- Fraud detection capability
- Precision
- Recall
- Generalization performance


---

# 🔍 Explainable AI

The system uses SHAP to explain model decisions.


Example explanations:

- Which features increased fraud probability
- Which features reduced risk
- Feature contribution ranking


SHAP provides transparency and improves trust in AI-based financial decisions.


# 🛠️ Tech Stack


## Programming

- Python


## Machine Learning

- Scikit-Learn
- Random Forest
- XGBoost
- Imbalanced-Learn


## Data Processing

- Pandas
- NumPy


## Explainable AI

- SHAP


## Backend

- Flask


## Frontend

- HTML5
- CSS3
- JavaScript


## Deployment

- Gunicorn
- Render


---

# 📂 Project Structure


```
Credit_Card_Fraud_Detection/

│
├── app.py
├── config.py
├── requirements.txt
├── Procfile
├── README.md
│
├── models/
│   ├── fraud_model.pkl
│   ├── scaler.pkl
│   └── explainer.py
│
├── src/
│   └── feature_mapper.py
│
├── reports/
│   └── explainability/
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
└── templates/
    └── index.html

```

---

# 🚀 Installation & Setup


## Clone Repository

```bash
git clone https://github.com/yourusername/Credit_Card_Fraud_Detection.git
```


## Navigate Into Project

```bash
cd Credit_Card_Fraud_Detection
```


## Create Virtual Environment

```bash
python -m venv venv
```


Activate:

Windows:

```bash
venv\Scripts\activate
```


Linux/Mac:

```bash
source venv/bin/activate
```


## Install Dependencies

```bash
pip install -r requirements.txt
```


## Run Application

```bash
python app.py
```


Open:

```
http://127.0.0.1:5000
```

---

# 🌐 Deployment

The application can be deployed using:

- Render
- AWS
- Azure
- Docker


Production server:

```
gunicorn app:app
```

---

# 🔮 Future Improvements

Future enhancements:

- Real-time transaction streaming
- Deep learning fraud detection
- User authentication
- Database integration
- Automated fraud alerts
- Advanced SHAP interactive dashboard
- Cloud deployment with monitoring


---

# 👨‍💻 Author

**Krishna Rajoo**

Machine Learning | Artificial Intelligence | Full Stack ML Applications


---

# ⭐ If You Like This Project

Give it a star ⭐ and feel free to explore, improve, and build upon it.
