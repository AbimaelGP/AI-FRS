# AI-FRS: An Ensemble-Based AI Decision-Support System for Fetal Risk Prediction

## Overview
AI-FRS (Artificial Intelligence–Fetal Risk Prediction System) is a clinical decision-support tool designed to classify fetal conditions as healthy or at risk using real-world obstetric data from a Mexican clinical setting. 

This system addresses a critical global health problem, where nearly 2 million stillbirths occur annually, often associated with limited healthcare resources and delayed risk detection. AI-FRS aims to support timely and informed clinical decisions through robust machine learning methodologies.

## Methodology
The proposed system is based on a **Two-stage ensemble learning strategy**:

- **7 base machine learning models**:
  - ANN, CNN, DT, RF, XGBoost, CatBoost, LightGBM  
- **127 first-order ensemble combinations** evaluated using hard voting  
- **32,752 second-order ensemble combinations** constructed from top-performing models  
- Selection based on **precision, recall, and F1-score**

The final model, referred to as **BSOEM (Best Second-Order Ensemble Model)**, achieved:

- **F1-score: 0.812**
- Improved balance between sensitivity and specificity
- Greater robustness compared to individual models and simple ensembles

Additionally, interpretability techniques were applied to identify the most influential clinical variables, enhancing transparency and clinical trust.

## System Architecture

### Ensemble Learning Strategy
![Ensemble Architecture](Fig1.png)

The system follows a two-stage ensemble process:
1. Generation and evaluation of first-order ensembles  
2. Construction of second-order ensembles using top-performing combinations  

This hierarchical approach significantly improves predictive performance and stability.

### Clinical Decision-Support Interface
![GUI System](Fig2.png)

AI-FRS includes a **user-friendly graphical interface** that allows clinicians to:

- Input patient clinical features  
- Obtain real-time fetal risk classification  
- Visualize:
  - Final prediction (Healthy/Risky)
  - Model voting behavior  
  - Risk probability score  

## Key Contributions
- Novel **ensemble-of-ensembles framework** for fetal risk prediction  
- Extensive evaluation of **32,752 model combinations**  
- Integration of **clinical interpretability**  
- Development of a **practical and deployable GUI tool**  

## Repository Status
The dataset will be made available upon registration and approval.  
This repository currently provides a description of the methodology and system.

## Authors
- Abimael Guzman-Pando  
- Bernardo O. Enriquez-Guillen  
- Graciela Ramirez-Alonso  
- Javier Camarillo-Cisneros  
- Cesar R. Aguilar-Torres  
- Luis C. Hinojos-Gallardo  
