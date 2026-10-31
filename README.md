
# Lightweight Mortar Strength Prediction Using ANN and NSGA-II

## Project Overview

This project investigates the use of Artificial Neural Networks (ANN) and the Non-dominated Sorting Genetic Algorithm II (NSGA-II) for predicting and optimizing lightweight mortar compressive strength.

The study extends an earlier linear regression and Genetic Algorithm approach by exploring nonlinear predictive modeling and multi-objective optimization.

## Objectives

- Investigate the relationship between mortar density, curing age, and compressive strength.
- Compare linear regression and ANN prediction models.
- Evaluate model performance using statistical metrics.
- Apply NSGA-II to explore trade-offs between mortar density and predicted compressive strength.
- Incorporate prediction uncertainty into the optimization process.

## Dataset

The research involves 500 experimental observations.

Input features:
- Mortar density (kg/m³)
- Curing age (days)

Target:
- Compressive strength (MPa)

Curing ages: 42, 48, 52, and 54 days.

The original experimental dataset is not publicly included.

## Methodology

### 1. Data Preprocessing
- Data validation and cleaning
- Descriptive statistical analysis
- Outlier and influential observation assessment
- Data splitting and feature scaling

### 2. Predictive Modeling
- Linear Regression
- Artificial Neural Networks (ANN)
- ANN architecture comparison

### 3. Model Evaluation
- R²
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Hold-out evaluation
- Repeated stratified cross-validation

### 4. Multi-Objective Optimization
- ANN ensemble surrogate modeling
- NSGA-II optimization
- Density minimization
- Predicted compressive strength maximization
- Uncertainty-aware Pareto optimization

## Reported Model Comparison

The accompanying research results workbook reports:

| Metric | Linear Regression | ANN |
|---|---|---|
| R² | 0.5571 | 0.6847 |
| MAE (MPa) | 0.1033 | 0.0873 |
| RMSE (MPa) | 0.1291 | 0.1089 |

These results are from the supplied research workbook.
The revised notebook may produce different results when re-executed.

## Technologies

- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- SciPy
- Pymoo
- Google Colab

## How to Run

1. Open the notebook in Google Colab.
2. Install the required dependencies.
3. Provide the authorized input dataset.
4. Update the dataset path if necessary.
5. Run the cells sequentially.
6. Review model evaluation and Pareto optimization results.

The notebook expects `Fitness_Function_Bersih.xlsx`
with a worksheet named `Data_Mentah`.

## Limitations

- Original experimental data are subject to research permissions.
- Model predictions depend on the experimental dataset.
- The revised notebook results require independent execution and verification.
- Optimized solutions require engineering validation before practical application.

## Project Information

**Year:** 2026

**Project Type:** Independent Research Collaboration

**Fields:** Machine Learning, Predictive Modeling, Civil Engineering, Multi-Objective Optimization

## My Contributions

- ANN model development and evaluation
- Comparison of linear and nonlinear prediction approaches
- NSGA-II optimization workflow
- Research data analysis and result interpretation
