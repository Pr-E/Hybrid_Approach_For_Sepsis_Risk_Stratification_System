# Hybrid_Approach_For_Sepsis_Risk_Stratification_System
MSc. Data Science Project

## Project Overview
This project aims to develop an advanced sepsis risk stratification model for ICU patients using a hybrid advanced machine learning approach. By integrating the PIRO (Predisposition, Infection, Response, Organ Dysfunction) scoring system with machine learning models like Long Short-Term Memory (LSTM) networks, Random Forest (RF), and eXtreme Gradient Boosting (XGBoost), this model enhances the early detection and accurate risk stratification of sepsis. The goal is to improve patient outcomes by enabling timely interventions and reducing healthcare costs.

## Features

- **Hybrid Model Architecture**: Combines LSTM for time-series feature extraction with RF and XGBoost for classification.
- **PIRO Scoring System Integration**: Uses the PIRO framework to incorporate multiple clinical dimensions for personalized sepsis risk assessment.
- **Time-Series Analysis**: Utilises LSTM networks to capture temporal patterns in patient data, crucial for understanding sepsis progression.
- **Evaluation Metrics**: Assesses model performance using confusion matrices, AUROC, sensitivity, specificity, and Decision Curve Analysis (DCA).
- **Clinical Applicability**: Designed to support healthcare providers in making informed decisions regarding sepsis management.

## Dataset

The dataset used in this project is sourced from Kaggle and contains simulated data from the first 24 hours of ICU hospitalisation for 200 patients with sepsis. The dataset includes 98 variables, out of which 18 were identified as relevant for the PIRO framework and used in the model. These 18 variables include:

- **Demographic Information**:
  - Sex
  - Age
- **Comorbidities**:
  - Diabetes Mellitus Type 2
  - Chronic Kidney Disease
  - Coronary Artery Disease
  - Autoimmune Disease
- **Infection Indicators**: Infection
- **Vital Signs**:
  - Systolic Blood Pressure
  - Heart Rate
  - Respiratory Rate
- **Laboratory Results**:
  - Lactate
  - White Blood Cell count (WBC)
  - C-reactive protein (CRP)
  - Procalcitonin (PCT)
- **Sepsis Severity**: Sequential Organ Failure Assessment (SOFA) Score
- **Outcomes**: Death
  
These variables were carefully selected based on their relevance to the PIRO framework to ensure accurate and personalised sepsis risk stratification.

## Installation

To run this project, you need to set up your environment with the following dependencies:

- Python 3.x
- PyTorch
- Scikit-learn
- pandas
- numpy
- matplotlib
- seaborn
- imbalanced-learn
- joblib

You can install the required libraries using the following command:

```bash
pip install torch scikit-learn pandas numpy matplotlib seaborn imbalanced-learn joblib
```
## Usage

To use this project, follow the steps below:

1. **Clone the Repository:**

   Clone the repository from GitHub to your local machine:

   ```bash
   git clone https://github.com/Pr-E/Hybrid_Approach_For_Sepsis_Risk_Stratification_System.git
   cd Hybrid_Approach_For_Sepsis_Risk_Stratification_System

2. **Run the Jupyter Notebook:**

   Open the provided Jupyter notebook (sepsis_risk_stratification.ipynb) to explore the data preprocessing, feature engineering, model training, and evaluation steps.

3. **Test the Model:**

   You can test the model on new patient data by following the steps outlined in the notebook. Simply replace the example data with your dataset and run the cells to see the model's predictions.
