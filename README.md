# Diabetes Prediction Using Support Vector Machine

## Overview
This project implements a machine learning pipeline to predict whether a patient is diabetic or non-diabetic based on diagnostic medical measurements. The model is trained using the **PIMA Indians Diabetes Dataset** and employs a **Support Vector Machine (SVM)** classifier with a linear kernel.

The notebook demonstrates the complete workflow of a supervised machine learning project, including data analysis, preprocessing, feature standardization, model training, evaluation, and real-time prediction.

---

## Dataset
- **Name:** PIMA Indians Diabetes Dataset
- **Source:** Publicly available medical dataset
- **Target Variable:** `Outcome`
  - `1` → Diabetic
  - `0` → Non-diabetic

---

## Project Workflow
1. Data Loading and Exploration  
2. Statistical Analysis  
3. Feature–Label Separation  
4. Feature Standardization  
5. Train–Test Split (Stratified)  
6. Model Training using SVM  
7. Model Evaluation (Accuracy Score)  
8. Predictive System Implementation  

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn

---

## Data Preprocessing
- The dataset is analyzed for statistical consistency.
- Features are standardized using `StandardScaler` to ensure uniform scaling.
- Stratified splitting is used to maintain class balance between training and testing sets.

---

## Model Training
- Algorithm: **Support Vector Machine (SVM)**
- Kernel: **Linear**
- The model is trained on 80% of the dataset and tested on the remaining 20%.

---

## Model Evaluation
- Accuracy is calculated for both training and testing datasets.
- Results indicate that the model is neither overfitted nor underfitted, demonstrating good generalization performance.

---

## Predictive System
The notebook includes a predictive system that accepts new patient data, reshapes it appropriately, applies standardization, and outputs a prediction indicating whether the patient is diabetic or not.

Example input:
```python
(3, 158, 76, 36, 245, 31.6, 0.851, 28)
```
---
## Results
- The trained SVM classifier achieves reliable accuracy on unseen data. (Above 75% accuracy for both Training and Testing)
- The project successfully demonstrates an end-to-end machine learning workflow suitable for beginner to intermediate practitioners.

---

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
2. pip install -r requirements.txt
3. jupyter notebook DiabetesPrediction_rbmlprjct.ipynb
