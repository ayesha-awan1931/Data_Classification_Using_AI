# 🌸 Iris Flower Classification Using Machine Learning

**DecodeLabs — Artificial Intelligence Internship, Project 2: Data Classification Using AI**
Batch 2026 · Supervised Learning Track

## Overview
This project implements a complete, end-to-end supervised machine learning pipeline that
classifies iris flowers into one of three species (*Setosa*, *Versicolor*, *Virginica*)
based on four physical measurements: sepal length, sepal width, petal length, and petal width.

## Dataset
- **Source:** Iris dataset, loaded directly via `sklearn.datasets.load_iris()`
  (equivalent to the classic UCI Machine Learning Repository Iris dataset).
- **Samples:** 150 (50 per class — perfectly balanced)
- **Features:** 4 numeric measurements (cm)
- **Target:** 3 species classes

## Project Structure
```
.
├── Iris_Classification_Project2.ipynb   # Main notebook (run this)
├── README.md                             # This file
├── requirements.txt                      # Python dependencies
├── class_distribution.png                # Generated on run
├── correlation_heatmap.png               # Generated on run
├── pairplot.png                          # Generated on run
├── accuracy_comparison.png               # Generated on run
├── confusion_matrix.png                  # Generated on run
├── roc_curve.png                         # Generated on run
└── feature_importance.png                # Generated on run
```

## How to Run
1. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate    # Windows: venv\Scripts\activate
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch Jupyter and run the notebook top to bottom:
   ```bash
   jupyter notebook Iris_Classification_Project2.ipynb
   ```
   The notebook is self-contained — it installs any missing libraries automatically and
   requires no external file downloads or manual edits.

## Pipeline Summary
1. Load & explore the dataset
2. Clean data (missing values, duplicates, outlier check)
3. Select features & encode the target label
4. Train/test split (80/20, stratified, reproducible)
5. Scale features with `StandardScaler`
6. Train and compare 6 classifiers: KNN, Logistic Regression, Decision Tree,
   Random Forest, Naive Bayes, SVM
7. Automatically select the best model by test accuracy
8. Evaluate with confusion matrix, classification report, precision, recall,
   F1 score, and multi-class ROC/AUC curves
9. Report feature importance and a full conclusion

## Report Outline (for submission writeup)
1. Title & Objective
2. Dataset Description & Justification
3. Data Preprocessing Steps
4. Model Selection Rationale
5. Training & Evaluation Methodology
6. Results (metrics + visualizations)
7. Discussion of Strengths / Weaknesses
8. Future Improvements
9. Conclusion

## Author
AI Intern — DecodeLabs, Batch 2026
Contact: decodelabs.tech@gmail.com · www.decodelabs.tech
