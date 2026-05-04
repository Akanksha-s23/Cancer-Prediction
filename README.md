# Cancer-Prediction
# Overview

  This project implements a machine learning model to predict whether a tumor is malignant (cancerous) or benign (non-cancerous) using features extracted from       cell nuclei. The goal is to build an accurate and interpretable classification system using supervised learning techniques.

# Dataset
  Source: YBI Foundation Cancer Dataset
  Contains numerical features such as:
 1 Radius
 2 Texture
 3 Perimeter
 4 Area
 5 Smoothness
  # Target variable:
    M (Malignant) → 1
    B (Benign) → 0
# Methodology
  Data Preprocessing
  Removed irrelevant columns (e.g., ID)
  Converted categorical labels into numerical values
  Feature Scaling
  Applied StandardScaler to normalize feature values
  # Model Used
    Logistic Regression (suitable for binary classification)
    Train-Test Split
    80% training and 20% testing data
# Results
  🔹 Accuracy
      97.36%
  🔹 Confusion Matrix
      [[70  1]
       [ 2 41]]
  🔹 Classification Performance
      Class	Precision	Recall	F1-Score
      Benign (0)	0.97	0.99	0.98
      Malignant (1)	0.98	0.95	0.96
# Interpretation
  The model performs very well overall, achieving high accuracy and balanced performance.
  High recall (0.95) for malignant cases indicates that most cancer cases are correctly identified.
  Only 2 cancer cases were missed, showing strong reliability.
  Precision for malignant class (0.98) suggests very few false alarms.
# Limitations
  The model only predicts malignant vs benign, not specific cancer types.
  Performance may vary with different datasets.
  Not intended for real-world medical diagnosis.
# Future Improvements
  Implement advanced models (Random Forest, XGBoost)
  Perform hyperparameter tuning
  Improve recall further to minimize missed cancer cases
  Use larger and more diverse datasets
# Technologies Used
  Python
  Pandas, NumPy
  Scikit-learn
  Matplotlib, Seaborn
# Conclusion
  This project demonstrates how machine learning can be effectively used for medical data classification. With an accuracy of over 97%, the model shows strong       potential as a decision-support tool in healthcare analytics.
