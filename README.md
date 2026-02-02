# CardioSense-AI  
### Explainable Cardiovascular Risk Prediction from Wearable ECG Data

## Project Overview
CardioSense-AI is an end-to-end machine learning pipeline for **early cardiovascular risk detection** using **wearable-style ECG data**.  
The project focuses on **clinically valid feature extraction**, **explainable AI**, and **robust handling of real-world physiological constraints**, aligning with research-to-product workflows in applied healthcare AI.

The system processes raw ECG signals, extracts **Heart Rate Variability (HRV)** features using short-time windows, and trains interpretable machine learning models to distinguish between **normal and abnormal cardiac rhythms**.

---

## Key Objectives
- Develop an **ECG-based predictive model** for cardiovascular abnormality detection  
- Simulate **wearable data conditions** using short ECG windows  
- Apply **Explainable AI (XAI)** to support clinical trust  
- Ensure **reproducibility, transparency, and regulatory awareness**

---

## Technical Highlights
- **Signal Processing**: ECG preprocessing, R-peak detection, window-based segmentation  
- **Feature Engineering**: Time-domain HRV features (SDNN, RMSSD, MeanNN, SDSD, pNN50)  
- **Machine Learning**: Logistic Regression and Random Forest classifiers  
- **Evaluation**: AUC-ROC, precision, recall, class imbalance awareness  
- **Explainability**: SHAP-based global and individual-level explanations  
- **Clinical Validity**: Removal of physiologically invalid HRV metrics for short windows  

---

## Results Summary
- **Logistic Regression AUC-ROC**: ~0.997  
- **Recall (abnormal class)**: 1.00  
- **Precision (abnormal class)**: 0.96  

These results demonstrate strong class separation while prioritizing **sensitivity for abnormal rhythms**, which is critical for early detection scenarios.

---

## Explainability & Trust
SHAP analysis shows that **reduced HRV variability metrics** (SDNN, RMSSD) are the dominant contributors to abnormal predictions, aligning with established clinical knowledge on autonomic dysfunction and arrhythmia risk.

---

## Datasets
- **MIT-BIH Arrhythmia Database (PhysioNet)**  
  Used for ECG signal analysis and HRV feature extraction  
- Public, de-identified datasets only (GDPR-safe)

---


