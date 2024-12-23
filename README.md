# Parameter Optimization in SVM

This project implements parameter optimization for Support Vector Machines (SVM) using different kernels to achieve the best accuracy on a dataset. The optimization involves evaluating combinations of hyperparameters (`C` and `gamma`) across multiple train-test splits to identify the best-performing kernel and hyperparameter set.

---

## Features

1. **Dataset Analysis**:
   - Handles missing values.
   - Removes irrelevant columns like `Date` and `Time`.
   - Visualizes the target variable distribution.

2. **SVM Optimization**:
   - Evaluates different SVM kernels: `linear`, `poly`, `rbf`, and `sigmoid`.
   - Uses a fitness function to measure SVM performance on accuracy.
   - Performs optimization across multiple train-test splits.

3. **Learning Curve**:
   - Visualizes the training and cross-validation accuracy across varying training set sizes to assess model performance and overfitting.

---

## Technologies Used

- **Languages**: Python
- **Libraries**:
  - `pandas`, `numpy`: Data manipulation
  - `matplotlib`, `seaborn`: Visualization
  - `scikit-learn`: Machine learning and evaluation

---

## Dataset

- The dataset used for this project is `Room_Occupancy_Data.csv`.
- Target Variable: `Room_Occupancy_Count`.

---

## Optimization Results

The performance results for each train-test split are summarized below:

| S. No. | Best Accuracy | Best Kernel | Best Nu (`C`) | Best Epsilon (`gamma`) |
|--------|---------------|-------------|---------------|-------------------------|
| 1      | 0.99          | linear      | 3.06          | 1.44                   |
| 2      | 0.99          | linear      | 3.20          | 3.52                   |
| 3      | 0.99          | poly        | 2.38          | 6.07                   |
| 4      | 1.00          | linear      | 4.96          | 2.06                   |
| 5      | 1.00          | linear      | 0.77          | 3.76                   |
| 6      | 1.00          | linear      | 0.42          | 9.85                   |
| 7      | 0.99          | linear      | 5.85          | 5.16                   |
| 8      | 0.99          | poly        | 8.11          | 1.52                   |
| 9      | 0.99          | poly        | 8.91          | 5.05                   |
| 10     | 0.99          | linear      | 8.34          | 3.46                   |

---
