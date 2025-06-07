# Task-7-Support-Vector-Machines-SVM-

1. Dataset:
Used Bank Customer Churn dataset (from Kaggle) with Exited as the binary target (1 = churn, 0 = stayed).

2. Tools & Libraries:
pandas, NumPy, Matplotlib, Seaborn, scikit-learn, imblearn.

3. Data Cleaning:
Removed rows with only a few missing values and dropped non-informative columns (RowNumber, CustomerId, Surname).

4. Encoding:

* Gender: Binary Encoding

* Geography: Frequency Encoding

5. Scaling:
Used StandardScaler to normalize features — important for SVM performance.

6. Initial Modeling:
Trained SVM with both linear and rbf kernels. Linear SVM failed to detect minority class (churners).

7. Class Imbalance Handling:
Applied class_weight='balanced' in SVM to improve recall and F1-score for churners.

8. Hyperparameter Tuning:
Used GridSearchCV to tune C and gamma with cross-validation for best model selection.

9. Dimensionality Reduction & Visualization:
Applied PCA (n_components=2) to visualize decision boundaries before and after tuning.

10. Performance Evaluation:
Evaluated models using confusion matrix, classification report (precision, recall, f1-score) — showed significant improvement after tuning and class balancing.
