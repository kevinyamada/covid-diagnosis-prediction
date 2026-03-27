# COVID 19 Diagnosis Prediction

This project compares a full prediction model and a practical screening model for classifying COVID 19 status using symptom and clinical data.

## Overview
We evaluated multiple models, including logistic regression, decision trees, and random forest, and selected a regularized logistic regression approach after it achieved the strongest final Kaggle performance.

## What the project does
- Predicts COVID 19 status from patient symptom data
- Compares a full feature model against a practical symptom-based model
- Handles intentionally flipped training labels using repeated out of fold prediction checks
- Tunes classification thresholds to study the tradeoff between accuracy, recall, and specificity

## Methods
- Logistic regression with glmnet
- Decision tree
- Random forest
- Feature engineering:
  - count features
  - threshold indicators
  - nonlinear terms
  - interaction terms
- 5-fold cross-validation
- Threshold tuning for screening performance

## Key Results
- Best final Kaggle score: 0.95208
- Full model OOF accuracy: 0.7653
- Practical model recall at threshold 0.34: 0.9028

## Files
- `STA314-Project.qmd`: analysis and code
- `report/STA314_Report.pdf`: final written report

## Notes
This project was completed as a course project with teammates.
