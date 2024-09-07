# MLSC_project_part1
Project Overview
The NASA NEO dataset contains information about asteroids and comets that come close to Earth's orbit. This project aims to predict if an NEO is hazardous based on features like orbital parameters, physical characteristics, and observation data.

Goals:
Perform data preprocessing (feature selection, encoding, normalization).
Handle class imbalance in the target column is_hazardous.
Build a machine learning model to classify hazardous and non-hazardous objects.
Dataset
The dataset used for this project includes details about:

Orbital parameters (e.g., semi-major axis, eccentricity, inclination).
Physical characteristics (e.g., size, rotation).
Observation data.
The target variable is the is_hazardous column, which indicates whether the NEO is classified as hazardous.
Modeling Process
The process involves:

Data Preprocessing:

Encoding categorical variables using one-hot encoding.
Scaling numerical features using standardization.
Feature selection based on correlation or feature importance.
Train/Test Split: The data is split into training and test sets (70/30 split).

Model Selection: A Random Forest classifier is used for prediction.

Handling Imbalanced Classes:

SMOTE (Synthetic Minority Over-sampling Technique): Used to balance the dataset by oversampling the minority class.
Class Weight Adjustment: Higher weights are assigned to the minority class to reduce misclassification.

Handling Imbalanced Classes
The target variable is_hazardous is imbalanced, with fewer hazardous objects compared to non-hazardous ones. We handle this imbalance using:

SMOTE (Synthetic Minority Over-sampling Technique): Generates synthetic samples for the minority class (hazardous objects).
Class Weights: The Random Forest model uses class weights to focus more on the minority class.
Balanced Accuracy Metric: Evaluates the model's performance by considering both classes equally.
