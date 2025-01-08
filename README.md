# Heart Disease Prediction with Apache Spark and Random Forest

## Overview
This project aims to build a scalable and efficient machine learning pipeline to predict heart disease using large datasets. We leverage **Apache Spark**, a powerful big data processing library, and implement the **Random Forest algorithm** from scratch to build a predictive model. Key sections of the implementation include:

1. **Data Preprocessing**: Handle missing values, standardize features, and prepare the dataset for modeling.
2. **Custom Random Forest Algorithm**: Implement the algorithm without relying on MLlib, focusing on distributed computation using RDDs.
3. **Model Evaluation**: Calculate metrics such as accuracy, F1-score, precision, and recall.
4. **Visualization and Insights**: Generate insights from statistical summaries and distribution analysis of key features.

## Motivation
Heart disease is one of the leading causes of death worldwide. Early prediction can save lives by enabling timely medical intervention. However, handling large medical datasets can be computationally expensive. This project demonstrates how **big data technologies** like Spark can efficiently process and analyze large datasets to make accurate predictions while implementing the machine learning algorithm without using pre-built libraries like MLlib.

## Features
- **Big Data Processing:** Utilize Apache Spark for distributed data processing.
- **Custom Algorithm Implementation:** Build the Random Forest algorithm from scratch for classification tasks.
- **Scalability:** Handle datasets that are too large for traditional machine learning tools.
- **Efficient Computation:** Optimize operations for distributed environments.

## Tools and Technologies
- **Apache Spark**: Distributed data processing framework.
- **Python**: Programming language for implementation.
- **Jupyter Notebook**: Interactive environment for development and visualization.

## Dataset
The dataset used in this project contains 14 features commonly used to predict heart disease. Below is the description of each feature:

| Feature    | Description                                      |
|------------|--------------------------------------------------|
| `age`      | Age of the patient                              |
| `sex`      | Gender (1 = male; 0 = female)                   |
| `cp`       | Chest pain type (4 values representing severity)|
| `trestbps` | Resting blood pressure (mm Hg)                  |
| `chol`     | Serum cholesterol (mg/dl)                       |
| `fbs`      | Fasting blood sugar (> 120 mg/dl, 1 = true; 0 = false) |
| `restecg`  | Resting electrocardiographic results (values 0, 1, 2) |
| `thalach`  | Maximum heart rate achieved                     |
| `exang`    | Exercise-induced angina (1 = yes; 0 = no)       |
| `oldpeak`  | ST depression induced by exercise relative to rest |
| `slope`    | Slope of the peak exercise ST segment           |
| `ca`       | Number of major vessels (0-3) colored by fluoroscopy |
| `thal`     | Thalassemia (3 = normal; 6 = fixed defect; 7 = reversible defect) |
| `target`   | Diagnosis of heart disease (1 = presence; 0 = absence) |

Dataset details:
- **Source:** Publicly available medical datasets (e.g., UCI Machine Learning Repository).
- **Size:** Large enough to demonstrate Spark’s big data capabilities.
- **Features:** Includes both numerical and categorical data relevant to heart disease prediction.
- ## Usage
- **Data Preprocessing:** Clean and preprocess the dataset to make it suitable for machine learning.
- **Model Training:** Train the Random Forest classifier using the custom implementation.
- **Evaluation:** Evaluate model performance using metrics such as accuracy, precision, recall, and F1-score.
- **Visualization:** Use Jupyter Notebooks to visualize the results.

## Results
- The custom Random Forest model achieves high accuracy in predicting heart disease.
- Feature importance is analyzed to understand which attributes contribute most to the predictions.

## Future Work
- Experiment with other algorithms like Gradient Boosted Trees implemented from scratch.
- Extend the pipeline for real-time predictions using Spark Streaming.
- Deploy the model as a REST API for integration with medical applications.
