# 🏥 Predicting Patient Mortality  
### Production-Style ML System with Explainability

This project implements an **end-to-end machine learning system** to predict **patient mortality risk** using structured healthcare data.

The focus goes beyond model accuracy to emphasize **engineering discipline, evaluation rigor, and explainability**, making the system suitable for **real-world clinical decision support**.

---

## 🚀 Project Highlights

The system follows a **production-style ML workflow**:

- Offline experimentation with **multiple algorithms**
- **Metric-driven model selection**
- Promotion of a **single best-performing model** for inference
- **SHAP-based explainability** to support interpretability in healthcare settings

---

## 🎯 Problem Statement

Patient mortality prediction is a critical healthcare task where **early risk identification** can support:
- Clinical decision-making  
- Resource allocation  
- Preventive interventions  

### Key Challenges Addressed

- **Class imbalance** (mortality events are rare)
- **Model interpretability** in a regulated domain
- **Threshold selection** for precision–recall trade-offs
- **Generalization vs overfitting**

---

## 🧠 ML & Engineering Approach

### 📊 Data Analysis & Feature Understanding
- Exploratory data analysis of demographic and clinical features
- Correlation analysis to identify feature relationships
- Visualization-driven insight generation

---

### 🧪 Multiple Model Experimentation

To avoid bias toward a single approach, multiple algorithms were implemented and evaluated:

- Logistic Regression (baseline)
- Decision Tree
- Random Forest

All models share a **common interface**, enabling consistent training, evaluation, and comparison.

---

### 📈 Model Evaluation Strategy

- **F1-score** used as the primary metric to handle class imbalance
- Threshold-aware evaluation to balance **recall vs precision**
- Overfitting analysis using **training vs validation metrics**

---

### 🏗️ Model Selection & Promotion

- All candidate models are trained and evaluated offline
- The **best-performing model** is promoted to production
- Non-selected models remain available for future experimentation and retraining

---

### 🔍 Explainability (SHAP)

- SHAP values used to interpret feature impact
- Enables inspection of **why** predictions are made
- Improves trust and transparency in model outputs

---

## 📊 Explainability & Visualizations

The project includes the following artifacts:

- Correlation heatmaps
- Model performance comparisons
- Training vs validation curves
- SHAP feature importance and summary plots

These visualizations support:
- Model debugging
- Stakeholder trust
- Communication with non-ML audiences

---

## 🏗️ Production Considerations

### 🔄 Model Retraining
Models can be retrained periodically as new patient data becomes available to prevent performance degradation.

### 🎚️ Threshold Calibration
Decision thresholds are configurable to balance recall vs precision based on clinical risk tolerance.

### 🧠 Explainability
SHAP-based explanations enable inspection of feature contributions for individual predictions.

### ⚠️ Failure Modes & Risks
- Data drift due to changing patient demographics  
- Missing or noisy clinical inputs  
- Bias amplification if retraining data is skewed  

---

## 🛠️ Tech Stack

### Machine Learning
- Python  
- Scikit-learn  
- SHAP  
- NumPy, Pandas  

### Backend / Serving
- FastAPI  
- Pydantic  
- Joblib  

### Visualization
- Matplotlib  
- Seaborn  

---

## 💡 Why This Project Matters

This project demonstrates:
- Engineering-quality ML pipelines
- Responsible metric selection
- Production-style model promotion
- Interpretability-first ML design

It emphasizes **trust, transparency, and decision impact**, which are critical for healthcare and other high-risk domains.

---

