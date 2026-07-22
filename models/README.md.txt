# Trained Models

This folder contains the trained Machine Learning models used in the **Multiple Disease Prediction Using Machine Learning** project.

## Models Included

### 1. Decision Tree
**File:** `decision_tree_model.pkl`

- Algorithm: Decision Tree Classifier
- Purpose: Predicts diseases by learning decision rules from the training data.
- Advantages:
  - Easy to understand and interpret.
  - Fast prediction.
  - Handles both numerical and categorical features.

---

### 2. Random Forest
**File:** `random_forest_model.pkl`

- Algorithm: Random Forest Classifier
- Purpose: Predicts diseases using an ensemble of multiple decision trees.
- Advantages:
  - Higher accuracy than a single decision tree.
  - Reduces overfitting.
  - Provides robust predictions.

---

### 3. Support Vector Machine (SVM)
**File:** `svm_model.pkl`

- Algorithm: Support Vector Machine
- Purpose: Classifies patient data by finding the optimal decision boundary.
- Advantages:
  - Effective for high-dimensional datasets.
  - Performs well on complex classification tasks.

---

### 4. Neural Network
**File:** `neural_network_model.pkl`

- Algorithm: Multi-Layer Perceptron (MLP)
- Purpose: Learns complex patterns in medical data for disease prediction.
- Advantages:
  - Captures non-linear relationships.
  - Suitable for complex datasets.

---

### 5. Multi-Disease Prediction Model
**File:** `multi_disease_model.pkl`

- Algorithm: Multi-Output Random Forest
- Purpose: Simultaneously predicts multiple diseases for a patient.
- Diseases Predicted:
  - Diabetes
  - Heart Disease
  - Parkinson's Disease

---

### 6. Standard Scaler
**File:** `scaler.pkl`

- Purpose: Standardizes input features before prediction.
- Importance:
  - Improves model performance.
  - Ensures consistent preprocessing during inference.

---

## Usage

Load any saved model using Joblib:

```python
import joblib

model = joblib.load("models/random_forest_model.pkl")
```

Load the scaler:

```python
scaler = joblib.load("models/scaler.pkl")
```

## Note

All models were trained using the dataset provided in this project. The saved model files can be loaded directly for prediction without retraining.