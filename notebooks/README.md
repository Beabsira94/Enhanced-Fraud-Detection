# Notebooks Folder Overview

The `notebooks` folder contains a series of Jupyter notebooks that document the step-by-step execution of the various tasks associated with the project, focusing on data analysis, model building, explainability, and deployment. These notebooks serve as a detailed record of the project's progress, showcasing the techniques applied to detect and prevent fraud in e-commerce and banking transactions. Each notebook addresses a specific task, from data preprocessing to model training and evaluation, using state-of-the-art machine learning techniques.

## Task 1: Data Analysis and Preprocessing (EDA.ipynb)

The **EDA.ipynb** notebook handles the critical data analysis and preprocessing tasks. This notebook includes handling missing values, data cleaning (removing duplicates and correcting data types), and performing exploratory data analysis (EDA) through univariate and bivariate analysis. Additionally, IP addresses are converted into integer format and merged with geographic location data to enhance fraud detection. The notebook also covers feature engineering, such as creating time-based features like `hour_of_day` and `day_of_week`, and calculating transaction frequency and velocity. Finally, normalization, scaling, and categorical encoding are performed to prepare the data for model building.

## Task 2: Model Building and Training

In this section, a series of machine learning models are developed to detect fraud in both e-commerce and banking transaction datasets. The models include traditional approaches like Logistic Regression, Decision Trees, and Random Forests, as well as advanced models like Gradient Boosting, Multi-Layer Perceptron (MLP), and Long Short-Term Memory (LSTM) networks. This notebook also implements model training, test splits, and evaluation techniques such as precision, recall, F1-score, and AUC-ROC to compare model performance. MLOps practices like versioning and experiment tracking are implemented using MLflow to ensure reproducibility and optimization throughout the process.

## Task 3: Model Explainability

Model explainability is crucial for understanding and trusting machine learning outcomes. This task uses SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-agnostic Explanations) to provide insights into how the model makes predictions. The notebook covers generating SHAP summary plots, force plots, and dependence plots to explain the contribution of different features. Similarly, LIME is used to explain individual predictions, highlighting the importance of specific features in classifying transactions as fraudulent or non-fraudulent. This step ensures transparency and interpretability in the models.

## Task 4: Model Deployment and API Development

This task focuses on deploying the fraud detection model using a Flask API. A Python script is developed to serve the trained models via API endpoints, allowing real-time fraud detection for incoming transactions. Docker is used to containerize the Flask application, enabling easy deployment and scalability. A logging system is integrated to track incoming requests and detect potential fraud. This notebook ensures that the fraud detection model can be deployed seamlessly in real-world applications, providing businesses with an effective tool to mitigate fraud risks.

## Task 5: Dashboard Development with Flask and Dash

In the final task, an interactive dashboard is built using Dash, which is integrated with Flask to visualize key fraud detection insights. The dashboard provides an overview of the total transactions, detected fraud cases, and geographic fraud trends. It features visualizations such as line charts tracking fraud cases over time, bar charts comparing fraud rates across devices and browsers, and maps to analyze where fraud is occurring geographically. This dashboard enhances the user's ability to monitor fraud trends and respond promptly to emerging risks.
