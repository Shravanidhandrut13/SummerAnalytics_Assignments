# SummerAnalytics_Assignments
Summer Analytics Course by IIT Guwahati 2025

# 🧠 NHANES Age Group Prediction Challenge (Hackathon2)

This repository contains a complete solution for the **NHANES Age Group Prediction** hackathon. The goal is to build a classification model that predicts whether an individual is an **Adult (0)** or a **Senior (1)** using health and demographic data from the NHANES dataset.

---

## 🚀 Problem Statement

Given health survey data, build a machine learning model to classify individuals into two age groups:

- **Adult (0)**
- **Senior (1)**

**Challenges addressed**:
- Missing values  
- Categorical variables  
- Class imbalance  
- Feature alignment across train/test sets

**Evaluation Metric**: F1 Score

---

## ⚙️ Tech Stack

| Tool          | Purpose                           |
|---------------|-----------------------------------|
| **Python 3.x** | Core programming language         |
| **Pandas**     | Data manipulation                 |
| **NumPy**      | Numerical computations            |
| **Scikit-learn** | Model selection, CV, metrics     |
| **LightGBM**   | Fast gradient boosting model      |
| **Jupyter Notebook** | Interactive model development |

---

## 🏗️ Architecture Flow

### ML Pipeline Overview

```mermaid
graph TD
    A[Start] --> B(Load Train/Test Data)
    B --> C(Exploratory Data Analysis)
    C --> D(Data Cleaning)
    D --> E(Feature Engineering)
    E --> F(Align Train/Test Features)
    F --> G(Model Training - LightGBM)
    G --> H(Hyperparameter Tuning)
    H --> I(Predict on Test Set)
    I --> J(Generate submission.csv)
    J --> K[End]
