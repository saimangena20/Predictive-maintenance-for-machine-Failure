# Predictive-maintenance-for-machine-Failure

Project Overview
Developed an ML model for predictive maintenance using the AI4I 2020 dataset. The project demonstrates an end-to-end workflow, from data analysis and preprocessing with a scikit-learn pipeline to model training. The goal is to predict machine failures to minimize downtime and optimize maintenance.
An End-to-End Predictive Maintenance Project
This project is a practical demonstration of an end-to-end machine learning workflow for predictive maintenance. Using the AI4I 2020 Predictive Maintenance dataset, a synthetic but realistic dataset, I developed a model to predict machine failures before they occur. The primary goal is to shift maintenance from a reactive or time-based approach to a proactive, data-driven one, thereby reducing unplanned downtime and optimizing operational efficiency.

The project showcases a complete data science pipeline, from exploratory data analysis (EDA) and robust preprocessing to model training and performance evaluation using industry-standard metrics.

Methodology
1. Data Source
The project utilizes the AI4I 2020 Predictive Maintenance Dataset from Kaggle. This dataset simulates sensor readings from industrial machinery, including:

Numerical Features: Air temperature, process temperature, rotational speed, torque, and tool wear.

Categorical Feature: Product type (L, M, H).

Target Variable: A binary label indicating whether a machine failure occurred.

2. Exploratory Data Analysis (EDA)
My initial analysis revealed a critical detail: a significant class imbalance in the target variable, which is a common characteristic of real-world failure data. This insight guided my choice of evaluation metrics later in the project. The EDA also included visualizations to understand feature distributions and correlations, identifying potential relationships between sensor readings and machine failures.

3. Preprocessing and Modeling
To ensure a robust and reproducible workflow, I implemented a scikit-learn Pipeline. This pipeline handles all data preprocessing steps, including:

Feature Scaling: Using StandardScaler to normalize numerical features.

One-Hot Encoding: Converting the categorical Type feature into a numerical format for the model.

The model used is a Random Forest Classifier, an effective and versatile ensemble model well-suited for this type of classification problem.

4. Evaluation
Due to the class imbalance, simple accuracy is not a reliable metric. Therefore, the model was evaluated on:

Precision and Recall: To understand the model's performance on the minority "failure" class.

F1-Score: To provide a balanced measure of the model's predictive ability.

Confusion Matrix: A visualization of the model's predictions versus the actual outcomes, which clearly shows the number of false positives and false negatives.

5. Final Model Performance
The Random Forest Classifier achieved a strong F1-score, demonstrating its capability to identify rare machine failures effectively. The confusion matrix shows that the model is highly successful at correctly classifying normal operations while also identifying a substantial number of actual failure cases.
