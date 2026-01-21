# Decision Tree Classification Analysis

This directory contains an implementation of a **Decision Tree Classifier**, a non-parametric supervised learning method used for classification tasks.

## Dataset Overview

The model uses the `Social_Network_Ads.csv` dataset, which includes:

- **Features**:
  - `Age`: Age of the user.
  - `EstimatedSalary`: Estimated salary of the user.
- **Target**:
  - `Purchased`: Binary classification (0 = No, 1 = Yes).

## Implementation Steps

The implementation follows these key steps:

1.  **Data Preprocessing**:
    - Split the dataset into Training (75%) and Test (25%) sets.
    - Applied **Feature Scaling** (Standardization) to normalize Age and Salary.
2.  **Model Training**:
    - Used `sklearn.tree.DecisionTreeClassifier` with default parameters.
3.  **Prediction and Evaluation**:
    - Predicted outcomes for the test set.
    - Evaluated the model using a **Confusion Matrix** and **Accuracy Score**.
4.  **Visualization**:
    - Plotted decision boundaries for both training and test sets to visualize the tree-based classification regions.

## Results

The Decision Tree model achieved the following performance on the test set:

- **Accuracy**: 91%
- **Confusion Matrix**:
  - True Negatives: 62
  - False Positives: 6
  - False Negatives: 3
  - True Positives: 29
- The model successfully captures non-linear decision boundaries, partitioning the feature space into rectangular regions based on the demographic features.
