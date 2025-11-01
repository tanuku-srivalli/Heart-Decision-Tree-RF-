# Heart Disease Prediction using Tree-Based Ensemble Methods

## Project Overview

This project implements and analyzes **Decision Tree** and **Random Forest** classifiers to predict the presence of heart disease using a clinical dataset (commonly the UCI Heart Disease Dataset). The objective is to demonstrate proficiency in tree-based modeling, manage overfitting, interpret model decisions, and perform robust evaluation using cross-validation.

## Tools and Libraries

  * **Primary Algorithms:** Decision Tree Classifier, Random Forest Classifier (Ensemble Learning)
  * **Language:** Python
  * **Libraries:**
      * `pandas` and `numpy`: Data manipulation and numerical operations.
      * `scikit-learn`: Model training, splitting data, and evaluation (e.g., `DecisionTreeClassifier`, `RandomForestClassifier`, `cross_val_score`).
      * `matplotlib`: Visualization (Feature Importances).
      * `graphviz`: Decision Tree visualization.

## Key Steps and Results

### 1\. Decision Tree Analysis (Overfitting Control)

A single **Decision Tree Classifier** was trained to establish a baseline. We specifically demonstrated the effect of **overfitting** in an unconstrained tree and controlled this by limiting the tree's depth (`max_depth`).

  * The final Decision Tree structure was visualized using `graphviz`.

### 2\. Random Forest (Ensemble Modeling)

A **Random Forest Classifier** was trained, which is an **ensemble** of multiple decision trees. This model demonstrated superior generalization capabilities compared to the single, constrained Decision Tree.

### 3\. Feature Importance Interpretation

The Random Forest model was used to determine the relative importance of each clinical feature in predicting heart disease.

| Rank | Feature | Clinical Relevance |
| :--- | :--- | :--- |
| **1** | **`oldpeak`** | ST depression induced by exercise (the most influential factor). |
| **2** | **`age`** | Patient age, a fundamental risk factor. |
| **3** | **`trestbps`** | Resting Blood Pressure. |
| **4** | **`chol`** | Serum Cholesterol. |

### 4\. Robust Evaluation

The final model performance was rigorously assessed using **K-Fold Cross-Validation** to ensure the accuracy score is reliable and not dependent on a single train-test split.


## Code Structure Highlights

The code is structured into five distinct steps, mirroring the task guide:

1.  Setup and Data Loading.
2.  Train and Visualize Unconstrained Decision Tree.
3.  Implement Max Depth constraint to control Overfitting.
4.  Train Random Forest and Compare Performance.
5.  Extract and Plot Feature Importances (as seen in the project analysis).
6.  Evaluate final Random Forest model using Cross-Validation.

-----
