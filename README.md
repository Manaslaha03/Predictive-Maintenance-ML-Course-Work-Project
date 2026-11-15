# Predictive Maintenance and Machine Failure Diagnosis

### Machine Learning Project | AI4I 2020 Dataset

## Overview
This project develops a machine learning system for predictive maintenance using the AI4I 2020 Predictive Maintenance Dataset.

The project focuses on two objectives:
- **Binary Classification:** Predict whether a machine will experience a failure.
- **Multi-label Classification:** Identify the possible type of machine failure.

## Dataset
- Dataset: AI4I 2020 Predictive Maintenance Dataset
- Total observations: 10,000
- Failure observations: 339
- Failure rate: 3.39%

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Feature Engineering
Three physics-inspired features were constructed:

1. Temperature Difference: `Process Temperature - Air Temperature`
2. Mechanical Power: `Torque × RPM × 2π / 60`
3. Wear-Torque Interaction: `Tool Wear × Torque`

## Machine Learning Algorithms
The project compares:
- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)

Random Forest was selected as the final binary classification model.

## Model Performance

| Metric | Test Result |
|---|---:|
| PR-AUC | 0.875 |
| ROC-AUC | 0.984 |
| Precision | 0.814 |
| Recall | 0.838 |
| F1-score | 0.826 |

*Precision, recall and F1-score correspond to the F1-optimal threshold of 0.42.*

## Failure Diagnosis
Five failure modes are investigated:
- TWF — Tool Wear Failure
- HDF — Heat Dissipation Failure
- PWF — Power Failure
- OSF — Overstrain Failure
- RNF — Random Failure

The models perform strongly for HDF, PWF and OSF, while TWF and RNF remain challenging.

## Project Structure
- `predictive_maintenance.ipynb` — Main machine learning notebook
- `Project_Report.pdf` — Detailed project report
- `README.md` — Project documentation

## Limitations
- The dataset is synthetic.
- Rare failure modes have limited observations.
- Real-world industrial validation is required.

## Author
**Manas Laha**

Mathematics Student | Interested in Artificial Intelligence and Machine Learning
