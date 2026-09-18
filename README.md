# Heart Disease Predictive System

A machine learning project that predicts the presence of heart disease from patient clinical data, using the UCI Cleveland Heart Disease dataset. Includes data cleaning, exploratory data analysis, three classification models (KNN, Logistic Regression, Random Forest), and an interactive Tableau dashboard.

## Workflow
- `Data_clean_Tablue.ipynb` - converts the raw `processed.cleveland.data` file into a CSV, handles missing values, encodes categorical fields, engineers an age-group feature, simplifies the target to binary (disease present/absent), and produces a Tableau-ready dataset
- `EDA_uncover_patterns.ipynb` - exploratory data analysis to uncover patterns and relationships in the cleaned dataset
- `Knn_Model.ipynb` - K-Nearest Neighbors classifier
- `Predictions_Logistic.ipynb` - Logistic Regression classifier
- `Random.ipynb` - Random Forest classifier
- `Dashboard_Heart_Disease.twb` - interactive Tableau dashboard built on the cleaned dataset

## Model results
| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---|---|---|---|---|
| KNN (k=8) | 0.89 | 0.93 | 0.84 | 0.89 | 0.93 |
| Logistic Regression | 0.89 | 0.88 | 0.91 | 0.89 | 0.92 |
| Random Forest | 0.89 | 0.93 | 0.84 | 0.89 | 0.94 |

## Tech stack
- Python
- pandas / numpy
- scikit-learn (KNN, Logistic Regression, Random Forest, train/test split, metrics)
- matplotlib (confusion matrices, ROC curves)
- Jupyter Notebook
- Tableau (dashboard)

## Project structure
- `processed.cleveland.data` - original UCI Cleveland Heart Disease dataset
- `heart_disease.csv` - dataset converted to CSV with named columns
- `heart_disease_cleaned_enhanced.csv` - cleaned dataset with engineered features and binary target
- `heart_disease_for_tableau_final.csv` - dataset with human-readable category labels for Tableau
- `Dashboard_Heart_Disease.twb` - Tableau workbook
- `AE2 Assessment_Analystics.pdf` - assessment/analytics write-up for this project

## Getting started
```bash
git clone https://github.com/Anandhu336/Heart-Disease-Predictive-System.git
cd Heart-Disease-Predictive-System
pip install pandas numpy scikit-learn matplotlib jupyter
jupyter notebook
```
Run the notebooks in order: `Data_clean_Tablue.ipynb` first to generate the cleaned CSVs, then `EDA_uncover_patterns.ipynb`, followed by any of `Knn_Model.ipynb`, `Predictions_Logistic.ipynb`, or `Random.ipynb` to train and evaluate the models. Open `Dashboard_Heart_Disease.twb` in Tableau to explore the dashboard.
