# 🌊 AI-Powered River Flood Prediction
### *Safeguarding South Asia's River Basins with Machine Learning*

![AI](https://img.shields.io/badge/Tech-AI%20%26%20Machine%20Learning-blueviolet)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Status](https://img.shields.io/badge/Status-Completed-green)
![Focus](https://img.shields.io/badge/Focus-Disaster%20Mitigation-red)

> **Author:** Pritam Rawal  
> **Location:** Kathmandu, Nepal  
> **Domain:** Artificial Intelligence for Social Good

## 📌 Executive Summary
The Himalayan and Terai regions (spanning Nepal and India) face annual devastation from riverine flooding. This project implements an **AI-powered predictive system** designed to forecast flood events before they occur.

By training advanced algorithms on hydrological data—specifically **River Discharge ($m^3/s$)** and **Water Levels**—this system identifies critical overflow thresholds. It serves as a prototype for a scalable **Early Warning System (EWS)** capable of saving lives and protecting agriculture in the Indo-Nepal borderlands.

## 🔍 The AI Solution
**The Challenge:**
Standard weather reports only tell you *if* it will rain, not *if* the river will flood your specific area.

**The Solution:**
I built a supervised learning engine that correlates three complex data layers:
1.  **Hydrological Dynamics:** Real-time river flow and rainfall intensity.
2.  **Topographical Intelligence:** Elevation gradients and soil drainage capacity (Clay vs. Silt).
3.  **Societal Impact:** Population density mapping in flood-prone zones.

## 📊 The Dataset
* **Source:** [Flood Risk in India (Kaggle)](https://www.kaggle.com/datasets/s3programmer/flood-risk-in-india)
* **Context:** While the dataset focuses on Indian geography, the topographical features (monsoon-driven river swelling, silt-heavy soil) are highly representative of the wider South Asian context, including Nepal.
* **Volume:** 1,000 Geospatial Records.
* **Key Features:** `Rainfall_mm`, `Clay_Ratio`, `Elevation_m`, `Population_Density`.

## 🛠️ Methodology & Tech Stack
### 1. Exploratory Data Analysis (EDA)
Understanding the "Why" behind the floods:
* **Correlation Analysis:** Discovered a high positive correlation between `Clay Soil` types and flood retention (due to poor drainage).
* **Urban Impact:** Visualized how high `Population_Density` in low-elevation zones amplifies flood risk.

### 2. Model Selection
I evaluated three algorithms to maximize **Recall** (minimizing false negatives is crucial for safety):
* **Logistic Regression:** Baseline model.
* **Random Forest:** Selected for its ability to handle non-linear interactions between soil and rainfall.
* **XGBoost:** Tested for high-performance gradient boosting.

## 📈 Key Results
| Metric | Performance |
| :--- | :--- |
| **Accuracy** | **92%** (Random Forest) |
| **Recall** | **0.89** (High sensitivity to actual flood events) |
| **Key Insight** | Areas with **>150mm Rainfall** and **<50m Elevation** showed a 95% probability of flooding. |

## 🚀 Future Scope: The Nepal Connection
As a developer based in Kathmandu, my goal is to extend this project to address **Transboundary Flood Management**:
1.  **Koshi & Gandaki Integration:** Adapt the model to include river discharge data from the major basins shared by Nepal and India.
