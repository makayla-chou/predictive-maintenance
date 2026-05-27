# Predictive Maintenance Machine Learning Project

This project uses industrial sensor data to predict whether a machine is likely to fail. The goal is to build a machine learning pipeline that can identify failure risk from operating conditions such as temperature, rotational speed, torque, and tool wear.

The dataset is highly imbalanced: only 3.39% of samples represent machine failures. Because of this, accuracy alone is not a reliable evaluation metric. This project focuses more on recall and F2 score, since missed failures are more costly in a predictive maintenance setting.

## Project Overview

The project includes:

- Exploratory data analysis of industrial sensor data
- Class imbalance analysis
- Baseline model evaluation
- Random Forest model training
- Classification threshold optimization using F2 score
- Model comparison across Logistic Regression, Random Forest, and Gradient Boosting
- Feature importance analysis
- Simplified decision tree visualization for interpretability

## Dataset

This project uses the AI4I 2020 Predictive Maintenance Dataset.

The dataset contains 10,000 machine records with features such as:

- Air temperature
- Process temperature
- Rotational speed
- Torque
- Tool wear
- Machine failure label

The dataset is not included in this repository. To run the notebook locally, download the dataset and place the CSV file inside a local `data/` folder.

Expected local structure:

```text
predictive-maintenance-ml/
│
├── data/
│   └── ai4i2020.csv
│
├── notebooks/
│   └── predictive-maintenance.ipynb
│
├── visuals/
│
├── README.md
├── requirements.txt
└── .gitignore
