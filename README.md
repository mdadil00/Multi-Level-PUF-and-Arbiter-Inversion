# Multi-Level PUF Modeling & Arbiter Inversion

## 📌 Overview
This project explores the **modeling and inversion of Physically Unclonable Functions (PUFs)** using linear machine learning techniques.  
We analyze the structure of **Multi-Level PUFs (ML-PUFs)**, which combine two arbiter PUFs and use XOR-based logic to generate robust responses.  
Through feature engineering and constrained optimization, the project demonstrates both the **predictability** of ML-PUFs and the **feasibility of reverse-engineering** Arbiter PUF delay parameters.

---

## 📖 Abstract
This report explores the modeling and inversion of Physically Unclonable Functions (PUFs) using linear machine learning techniques. We begin by analyzing the structure of Multi-Level PUFs (ML-PUFs), which combine two arbiter PUFs and utilize XOR-based logic to generate more robust responses. Through careful feature engineering, we demonstrate how a linear model can be constructed to accurately predict ML-PUF responses by transforming input challenges into a higher-dimensional feature space. Additionally, we address the inverse problem of reconstructing delay parameters from a learned arbiter PUF model. We formulate this as a constrained optimization problem, recovering a valid set of non-negative delays consistent with the given linear weights. Experimental results validate the efficacy of our methods in both tasks, highlighting the surprising predictability of ML-PUFs and feasibility of reverse-engineering PUF characteristics from model parameters.

---

## 🚀 Key Features
- **Feature Engineering**: Designed a **105-dimensional feature map** using linear predictors with XOR delay features for ML-PUF modeling.  
- **High Accuracy**: Achieved **100% test accuracy** using LinearSVC and Logistic Regression with carefully tuned hyperparameters.  
- **Arbiter Inversion**: Inverted a **64-bit Arbiter PUF** by solving a **65×256 sparse system** under non-negativity constraints, recovering **256 hardware delay parameters**.  
- **Security Insights**: Demonstrated **PUF vulnerabilities** by achieving perfect prediction and validating inversion accuracy against simulations.

---

---

## ⚙️ Tech Stack
- **Languages**: Python  
- **Libraries**: scikit-learn, NumPy, SciPy, Matplotlib  
- **Models Used**: LinearSVC, Logistic Regression, Ridge Classifier  
- **Optimization**: Constrained optimization with non-negativity constraints  

---

## 📊 Results
- Perfect classification on ML-PUF challenge-response pairs using linear models.  
- Successful recovery of **256 hardware delay parameters** from Arbiter PUF inversion.  
- Demonstrated the **predictability and vulnerabilities** of ML-PUFs under machine learning attacks.  

---

## 🧑‍🏫 Course Context
- **Project**: CS771 – Machine Learning  
- **Instructor**: Prof. Purushottam Kar  
- **Institution**: IIT Kanpur  
- **Duration**: Feb’25 – Apr’25  

