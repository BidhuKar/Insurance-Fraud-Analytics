🕵️ Insurance Claim Fraud Detection using Machine Learning
A real-world project to detect fraudulent insurance claims using data analysis, feature engineering, and classification models in Python.

📌 Overview

Insurance fraud is a billion-dollar problem that increases premiums for honest customers and results in significant losses to companies. This project investigates and models fraudulent claim behavior using real-world data. The goal is to identify suspicious claims early and help fraud investigators focus efforts on high-risk cases.

The analysis includes:
	•	Data preprocessing and EDA
	•	Class balancing for imbalanced target classes
	•	Feature engineering (e.g., hobbies transformation, claim history)
	•	Training a LightGBM model for classification
	•	Model interpretation using feature importance

 🧠 Problem Statement

Can we build a machine learning model that can accurately classify whether a claim is fraudulent or genuine, using customer and claim metadata?

🗃️ Dataset
	•	Source: [Kaggle / Public Insurance Dataset]
	•	File: insurance_claims.csv
	•	Target column: fraud_reported (Y/N)
	•	Records: ~10,000
	•	Key Features: Customer occupation, claim amount, past history, policy binding dates, auto models, incident severity, injury details, etc.

 🔍 Exploratory Data Analysis (EDA)
	•	Plotted class distribution: Data is imbalanced (fraud cases are rare).
	•	Checked null values and types.
	•	Investigated correlations between features and the fraud label.
 
 💡 Results & Interpretation
	•	Top Predictors of Fraud:
	•	incident_severity
	•	insured_hobbies
	•	auto_make
	•	incident_location
	•	witness_present
	•	Visualized feature importance using LightGBM’s built-in tools.

✅ Business Impact

This fraud detection pipeline can:
	•	Save millions in illegitimate payouts.
	•	Help claims investigators prioritize cases.
	•	Reduce manual workload and investigation time.
	•	Integrate into real-time claim scoring systems.
	•	Created visual summaries using seaborn & matplotlib.

Key Insight: Certain hobbies, incident types, and claim amounts showed patterns differentiating fraud vs. non-fraud cases.
