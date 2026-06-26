# EV Charging Behaviour Prediction using Machine Learning

## Overview

This project aims to analyze and predict Electric Vehicle (EV) charging behaviour using Machine Learning techniques. The system identifies hidden charging patterns among EV users and predicts future charging demand based on temporal, environmental, and operational factors.

The project combines unsupervised learning for user persona discovery and supervised learning for charging demand prediction, enabling intelligent charging infrastructure management.

## Problem Statement

With the rapid adoption of Electric Vehicles, charging stations often experience:

Uneven utilization
Long waiting times
Peak-hour congestion
Inefficient energy distribution

Existing systems primarily react to demand rather than anticipating it.
This project addresses these challenges by learning EV charging behaviour and predicting future charging requirements.

## Objectives

Analyze EV charging patterns.
Discover hidden EV user personas using clustering.
Predict charging demand using machine learning models.
Identify key factors influencing charging behaviour.
Provide insights for smarter charging infrastructure planning.
Project Workflow
    ↓
Data Preprocessing
    ↓
Feature Engineering
    ↓
K-Means Clustering
(User Persona Discovery)
    ↓
Persona Assignment
    ↓
PCA Visualization
    ↓
Random Forest & XGBoost Models
    ↓
Charging Demand Prediction
    ↓
Model Evaluation

## Dataset Features

The dataset includes several attributes related to EV charging sessions, such as:

Charging Duration
Energy Consumed (kWh)
Initial Battery State of Charge (SOC)
Final Battery State of Charge (SOC)
Waiting Time
Charging Power
Queue Length
Weather Conditions
Traffic Density
Vehicle Type
Charging Location
Timestamp Information

Additional features engineered:

Hour of Day
Month
Day of Week
Weekend Indicator

## Machine Learning Techniques
1. K-Means Clustering
Used to identify hidden charging behaviour patterns among EV users.

Example personas discovered:

Home Chargers
Fast Chargers
Weekend Drivers
Peak-Hour Users

2. Random Forest Regressor
Used for predicting charging demand based on behavioural and environmental features.

3. XGBoost Regressor
Implemented to compare predictive performance with Random Forest.

Dimensionality Reduction

Principal Component Analysis (PCA) was applied to visualize user clusters in a lower-dimensional space.

Evaluation Metrics

The models were evaluated using:

Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score
Cross Validation

## Key Insights
Charging behaviour varies significantly across different user groups.
Temporal factors such as hour of day and weekends strongly influence charging demand.
Environmental and operational factors impact charging decisions.
User personas improve predictive performance.

## Technologies Used
Python
Pandas
NumPy
Scikit-learn
XGBoost
Matplotlib
Seaborn
Jupyter Notebook

## Project Structure
EV-Charging-Behaviour-Prediction/
│
├── EV_Charging_Behaviour_Prediction.ipynb
├── README.md
├── dataset/
├── images/
└── requirements.txt


## Results
The proposed framework successfully combines clustering and ensemble learning to model EV charging behaviour and predict charging demand with high accuracy.

The study demonstrates that integrating user persona discovery with predictive modelling can support intelligent EV charging infrastructure management.