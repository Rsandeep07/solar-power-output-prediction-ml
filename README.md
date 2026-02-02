# Solar Power Output Prediction – Phase 1

This repository contains **Phase 1** of a Machine Learning Capstone Project focused on predicting solar power output using historical generation data.

The project follows a structured, end-to-end machine learning workflow aligned with industry practices and mentor guidelines.

---

##  Project Overview

Solar power generation is inherently variable due to its dependence on environmental and operational factors.  
Accurate prediction of power output is crucial for efficient energy planning and monitoring of system performance.

The objective of this project is to build a machine learning solution that predicts **AC power output** of a solar plant using historical generation data.

---

##  Project Phases

### Phase 1: Problem & Data Foundations 
- Problem statement definition  
- Dataset selection and understanding  
- Target variable identification  
- Exploratory Data Analysis (EDA)  
- Evaluation metric definition  

### Phase 2: Modeling & Explainability *(upcoming)*
- Feature engineering  
- Multiple machine learning models  
- Hyperparameter tuning  
- Model interpretability  

### Phase 3: Deployment & MLOps *(upcoming)*
- Streamlit application  
- Hugging Face deployment  
- MLflow experiment tracking  
- Prefect pipelines  

---

##  Dataset

- **Source:** Kaggle – Solar Power Generation Data  
- **File Used:** `Plant_1_Generation_Data.csv`

The dataset contains inverter-level solar power generation data recorded at regular time intervals.

---

## 🎯 Target Variable

- **AC_POWER**

**Justification:**  
AC power represents the actual usable electricity delivered to the grid, making it a meaningful and business-relevant target variable for prediction.

---

##  Exploratory Data Analysis (EDA)

EDA was performed to understand data characteristics before modeling. The analysis focused on:
- Distribution of AC power values  
- Zero-value occurrences in power generation  
- Relationship between DC power and AC power  
- Time-based solar generation patterns  

### Key Observations:
- AC power is zero during night-time periods, which is expected for solar plants  
- A strong linear relationship exists between DC power and AC power  
- Solar generation follows a clear daily cycle, peaking around midday  

---

##  Evaluation Metrics

Since this is a regression problem, the following metrics are defined for model evaluation in later phases:
- **RMSE (Root Mean Squared Error)**  
- **R² Score**

These metrics will be consistently used during model comparison.

---

##  Repository Structure (Phase 1)

```text
solar-power-output-prediction-ml/
│
├── notebooks/
│ └── Phase_1_Problem_and_Data_Foundations.ipynb
│
├── README.md
```


---

##  Phase 1 Status

Phase 1 focuses exclusively on problem understanding and data exploration.  
No modeling, tuning, or deployment has been performed at this stage.

---

##  Next Steps

- Begin **Phase 2: Modeling & Explainability**
- Train and compare multiple machine learning models
- Introduce feature engineering and interpretability techniques

---

*This project is developed as part of a Machine Learning Capstone Project with a focus on industry-ready workflows and best practices.*

