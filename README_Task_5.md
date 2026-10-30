# Task 5 – Machine Learning Classification Model

## Project Overview

This project applies supervised machine learning techniques to classify Netflix titles as Movies or TV Shows using catalogue metadata.

Two classification algorithms, Logistic Regression and Random Forest, were trained and evaluated using Scikit-learn.

## Objectives

- Prepare features for machine learning.
- Split data into training and testing sets.
- Train classification models.
- Evaluate model performance.
- Compare model results and establish a baseline.

## Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- TF-IDF Vectorization
- Logistic Regression
- Random Forest

## Dataset

The project uses a cleaned Netflix dataset containing 8,790 records.

The target variable is `type`, which contains two classes:

- Movie
- TV Show

## Feature Engineering

The following features were used:

- `release_year`
- `rating`
- `country`
- `listed_in`

The text-based attributes were combined into a content feature and transformed using TF-IDF Vectorization. The release year was scaled using StandardScaler.

Duration-related features were excluded to avoid directly using a strong indicator of content type.

## Model Development

Two classification algorithms were implemented:

1. **Logistic Regression**
   - Trained with a maximum of 1,000 iterations.
2. **Random Forest Classifier**
   - Used 100 estimators.
   - Applied balanced class weights.

The dataset was divided into training and testing sets using an 80:20 split, with stratification and a random state of 42.

## Model Evaluation

| Model | Test Accuracy |
|---|---:|
| Logistic Regression | 100% |
| Random Forest | 100% |
| Most-Frequent-Class Baseline | 69.68% |

Both models correctly classified all 1,758 test records in the selected split.

Additional evaluation included:
- Classification reports
- Confusion matrices
- Comparison with a baseline classifier
- Examination of exact feature-combination overlap between training and testing data

## Important Model Limitation

Although both models achieved 100% test accuracy, this result should be interpreted cautiously.

The classification task uses catalogue metadata such as genre, country, and rating, which can strongly indicate whether a title is a Movie or TV Show.

The test data also comes from the same underlying dataset. Therefore, perfect accuracy on this split does not establish that the models will achieve similar performance on new, independently collected data.

## Key Learning Outcomes

- Supervised machine learning
- Feature engineering
- TF-IDF Vectorization
- Data preprocessing pipelines
- Train-test splitting
- Logistic Regression
- Random Forest Classification
- Model evaluation and comparison
- Understanding data leakage and generalization limitations

## Project File

- `task 5.ipynb` – Jupyter Notebook containing the complete classification workflow.

