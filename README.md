# Heart Disease Analysis (UCI Dataset)

This project applies machine learning techniques to predict the presence of heart disease using the UCI Heart Disease dataset. The workflow includes data exploration, preprocessing, feature encoding, model training, evaluation, and optimization.

A Decision Tree Classifier is used as the baseline model and further improved using hyperparameter tuning with GridSearchCV to achieve better generalization and prediction performance.

## Files
- `Heart-Disease-Analysis.ipynb` – Jupyter notebook with data analysis and model building
- `heart_disease_uci.csv` – Dataset used for analysis

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Objective

The objective of this project is to analyze patient medical data and build an optimized classification model that can accurately predict whether a patient has heart disease.

## Dataset Information

- Total Samples: 920  
- Features Used: 13  
- Target Variable: Presence of heart disease (Disease / No Disease)

## Model & Evaluation

### Baseline Decision Tree Performance
- Training Accuracy: **100%**
- Testing Accuracy: **76.09%**

**Classification Report (Test Set):**
- Precision: 0.76
- Recall: 0.76
- F1-Score: 0.76

This indicates slight overfitting in the baseline model.

### Optimized Decision Tree (GridSearchCV)

**Best Hyperparameters:**
- Criterion: `gini`
- Max Depth: `4`
- Min Samples Leaf: `10`
- Min Samples Split: `2`

**Final Model Performance:**
- Accuracy: **79.89%**
- Precision: **80.37%**
- Recall: **84.31%**
- F1-Score: **82.30%**

The optimized model shows improved performance and better generalization compared to the baseline model.

## Conclusion

The optimized Decision Tree model successfully predicts heart disease with improved accuracy and balanced evaluation metrics. This project demonstrates effective use of data preprocessing, model evaluation, and hyperparameter tuning in a real-world healthcare dataset.
