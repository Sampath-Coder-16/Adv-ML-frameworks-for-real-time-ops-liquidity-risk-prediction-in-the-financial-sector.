📊 Advanced ML Frameworks for Real-Time Bank Liquidity Risk Prediction
📌 Project Overview

This project presents a comprehensive comparative analysis of Machine Learning models for predicting Bank Liquidity Risk using financial and macroeconomic indicators.

The goal is to build an AI-driven early warning system that helps financial institutions and regulators detect liquidity stress before it becomes critical.

This study benchmarks multiple ML algorithms and identifies the most suitable model for real-world deployment.

🎯 Objectives

Develop an AI-based liquidity risk prediction system

Perform comparative analysis of multiple ML models

Handle class imbalance using up-sampling

Evaluate models using 13 performance metrics

Identify the best model for real-time regulatory monitoring

Create a dashboard-ready predictive framework

🏦 Dataset Information

Dataset Name: BankLiquidityRiskDetection.csv

Banks Covered: 38 Tanzanian banks

Time Period: 2010 – 2021

Target Variable: XX_MLA_CLASS2

Liquidity Risk Classes:

1 – Strong

2 – Satisfactory

3 – Fair

4 – Weak

5 – Critically Deficient

The dataset includes:

Bank-specific financial indicators

Macroeconomic variables

Regulatory metrics

🧹 Data Preprocessing Steps

Imported dataset into Pandas DataFrame

Checked shape, data types, summary statistics

Removed duplicates

Dropped irrelevant columns:

Unnamed: 0

REPORTINGDATE

INSTITUTIONCODE

Handled missing values:

Numerical → Median imputation

Categorical → Mode / New category

Standardized features using StandardScaler

⚖️ Handling Class Imbalance

The original dataset had severe class imbalance.

To address this:

Applied Up-Sampling (Random Resampling with Replacement)

Balanced all five MLA classes equally

Ensured unbiased model training

🧠 Feature Engineering

The following 8 engineered features were used:

Bank Size

GDP Growth

Loan-to-Assets Ratio

NPL Ratio

NPL Net of Provisions Ratio

NPLNP to Core Capital

Lending Rate

Liquid Assets to Total Assets (LATA)

A correlation matrix confirmed:

No severe multicollinearity

Features are statistically stable

🔬 Machine Learning Models Implemented

The following supervised ML algorithms were trained and compared:

Logistic Regression (LR)

Decision Tree (DT)

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Random Forest (RF)

Multi-Layer Perceptron (MLP)

XGBoost (XGB)

Hybrid RF–MLP Model

🔷 Hybrid RF–MLP Strategy

The hybrid model combines:

Random Forest predictions

MLP predictions

Selects the higher-risk output for enhanced safety

📊 Model Evaluation Metrics (13 Metrics)

Models were evaluated using:

Accuracy

Balanced Accuracy

Precision

Recall

F1-Score

Cohen’s Kappa

Area Under Curve (AUC)

Type I Error

Type II Error

G-Mean

Youden’s Index

Negative Likelihood Ratio (NLiR)

Discriminant Power

This ensures a comprehensive, unbiased performance comparison.

📈 Results Summary
🥇 Best Performing Models
Model	Test Accuracy	Performance
Hybrid RF–MLP	99.78%	Best overall
XGBoost	~99%	Excellent generalization
Random Forest	~98–99%	Highly stable
📌 Key Findings

Hybrid RF–MLP achieved top performance in:

Accuracy

Precision

Recall

F1-Score

Cohen’s Kappa (0.9967)

XGBoost showed strong generalization

Ensemble methods minimized:

Type I Errors (False Positives)

Type II Errors (False Negatives)

Linear models (LR) underperformed compared to ensemble models

📊 Performance Insights

AUC scores exceeded 99% for advanced models

Tree-based models handled nonlinear relationships better

Hybrid model balanced risk sensitivity and false-alarm control

Strong discriminative power between high-risk and low-risk banks

🏗️ Project Workflow

Define Research Objective

Load Dataset

Clean & Preprocess Data

Feature Engineering

Handle Class Imbalance

Train-Test Split (67% / 33%)

Train ML Models

Evaluate using 13 metrics

Select Best Model

Integrate into Risk Monitoring Dashboard

🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-learn

XGBoost

Matplotlib

Seaborn

📌 Real-World Applications

Early warning systems for banks

Regulatory supervision tools

Financial stability monitoring

Risk management dashboards

AI-based compliance systems

🏆 Conclusion

This project demonstrates that:

Ensemble and Hybrid ML models significantly outperform traditional models

Hybrid RF–MLP provides the most reliable and balanced liquidity risk detection

AI-driven monitoring systems can strengthen financial sector stability

The findings provide an evidence-based recommendation for regulators and banks to adopt ensemble AI models for liquidity risk supervision.

📚 References

Key research references include:

Machine Learning for Liquidity Risk Prediction

Deep Learning for Financial Stability

XGBoost in Banking Risk Modeling

AI-driven Early Warning Systems

(Refer to full reference list in the research paper)
