# Solar Power Output Prediction – Phase 1

This repository contains **Phase 1** of a Machine Learning Capstone Project focused on
predicting solar power output using historical generation and weather sensor data.

The project follows a **structured, end-to-end machine learning workflow**
aligned with **industry practices** and **mentor guidelines**.

---

## Project Overview

Solar power generation is inherently variable due to its dependence on
environmental and operational factors such as irradiance, temperature, and time of day.

Accurate prediction of power output is crucial for:
- Energy planning  
- Grid stability  
- Monitoring plant performance  

The objective of this project is to build a machine learning solution that predicts
**AC power output** of a solar plant using historical generation and weather data.

---

## Project Phases

### Phase 1: Problem & Data Foundations
- Problem statement definition  
- Dataset selection and understanding  
- Target variable identification  
- Exploratory Data Analysis (EDA)  
- Evaluation metric definition  

### Phase 2: Modeling & Explainability *(upcoming)*
- Feature engineering  
- Training multiple ML models  
- Hyperparameter tuning  
- Model interpretability  

### Phase 3: Deployment & MLOps *(upcoming)*
- Streamlit application  
- Hugging Face deployment  
- MLflow experiment tracking  
- Prefect pipelines  

---

## Dataset

- **Source:** Kaggle – Solar Power Generation Data  
- **Data Format:** Excel files (`.xlsx`)  

The project uses inverter-level **power generation data** along with
**weather sensor data**, recorded at regular time intervals.

### Files Included
- `Plant_1_Generation_Data.xlsx`  
- `Plant_1_Weather_Sensor_Data.xlsx`  
- `Plant_2_Generation_Data.xlsx`  
- `Plant_2_Weather_Sensor_Data.xlsx`  

The datasets represent **two solar plants**, each containing:
- Power generation data (DC power, AC power, yield)  
- Weather sensor data (environmental measurements)  

All raw datasets are stored in the `solar_power_prediction_data/` directory.

---

## Target Variable

- **AC_POWER**

### Justification
AC power represents the **actual usable electricity delivered to the grid**.
It is the most **business-relevant and operationally meaningful** target
for solar power output prediction.

---

## Exploratory Data Analysis (EDA)

EDA was performed to understand the data characteristics before modeling.
The analysis focused on:

- Distribution of AC power values  
- Zero-value occurrences in power generation  
- Relationship between DC power and AC power  
- Time-based solar generation patterns  

### Key Observations
- AC power is zero during night-time periods, which is expected for solar plants  
- A strong linear relationship exists between DC power and AC power  
- Solar generation follows a clear daily cycle, peaking around midday  

---

## Evaluation Metrics

Since this is a **regression problem**, the following metrics are defined
for model evaluation in later phases:

- **RMSE (Root Mean Squared Error)**  
- **R² Score**

These metrics will be consistently used for model comparison.

---

## Repository Structure (Phase 1)

```text
solar-power-output-prediction-ml/
│
├── solar_power_prediction_data/
│ ├── Plant_1_Generation_Data.xlsx
│ ├── Plant_1_Weather_Sensor_Data.xlsx
│ ├── Plant_2_Generation_Data.xlsx
│ └── Plant_2_Weather_Sensor_Data.xlsx
│
├── notebooks/
│ └── Phase_1_Problem_and_Data_Foundations.ipynb
│
├── README.md
