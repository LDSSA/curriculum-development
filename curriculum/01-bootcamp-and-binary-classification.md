# S01 — Bootcamp and Binary Classification

S01 introduces the data-analysis, supervised-learning, and machine-learning workflow skills used throughout the Academy.

For the no-exam edition, SLU01–03 are regular S01 learning units. They are not admissions units. SLU01–17 are mandatory. SLU18, SLU19, SLU32, and SLU64 are optional.

## Curriculum overview

| Unit  | Name                                      | Core competency        | Presented at   | Required |
|-------|-------------------------------------------|------------------------|----------------|----------|
| SLU01 | Pandas 101                                | Data Skills & Analysis | Not presented  | Yes      |
| SLU02 | Subsetting Data in Pandas                 | Data Skills & Analysis | Not presented  | Yes      |
| SLU03 | Visualization with Pandas and Matplotlib  | Data Skills & Analysis | Not presented  | Yes      |
| SLU04 | Basic Statistics with Pandas              | Data Skills & Analysis | Bootcamp Day 1 | Yes      |
| SLU05 | Covariance and Correlation                | Data Skills & Analysis | Bootcamp Day 1 | Yes      |
| SLU06 | Dealing with Data Problems                | Data Skills & Analysis | Bootcamp Day 1 | Yes      |
| SLU07 | Linear Regression                         | Learning Algorithms    | Bootcamp Day 1 | Yes      |
| SLU08 | Metrics for Regression                    | ML Fundamentals        | Bootcamp Day 1 | Yes      |
| SLU09 | Logistic Regression                       | Learning Algorithms    | Bootcamp Day 1 | Yes      |
| SLU10 | Metrics for Classification                | ML Fundamentals        | Bootcamp Day 1 | Yes      |
| SLU11 | Tree-Based Models                         | Learning Algorithms    | Bootcamp Day 2 | Yes      |
| SLU12 | Feature Engineering                       | Data Skills & Analysis | Bootcamp Day 2 | Yes      |
| SLU13 | Bias–Variance Trade-off and Model Selection | ML Fundamentals      | Bootcamp Day 2 | Yes      |
| SLU14 | Model Complexity and Overfitting          | ML Fundamentals        | Bootcamp Day 2 | Yes      |
| SLU15 | Hyperparameter Tuning                     | ML Fundamentals        | Bootcamp Day 2 | Yes      |
| SLU16 | Workflow                                  | ML Fundamentals        | Bootcamp Day 2 | Yes      |
| SLU17 | Ethics and Fairness                       | Data Skills & Analysis | Bootcamp Day 2 | Yes      |
| SLU18 | Support Vector Machines                   | Learning Algorithms    | Not presented  | No       |
| SLU19 | k-Nearest Neighbors                       | Learning Algorithms    | Not presented  | No       |
| SLU32 | Training for Hackathon, Part 1            | Hackathon Preparation  | Not presented  | No       |
| SLU64 | Training for Hackathon, Part 2            | Hackathon Preparation  | Not presented  | No       |

## Competencies

### Data Skills and Analysis

Students learn to prepare, inspect, analyze, visualize, and communicate data with pandas and Matplotlib.

### Learning Algorithms

Students gain practical experience with linear regression, logistic regression, decision trees, ensemble models, support vector machines, and k-nearest neighbors.

### Machine-Learning Fundamentals

Students learn model evaluation, overfitting and underfitting, feature selection, regularization, hyperparameter tuning, reproducible workflows, and responsible model development.

## Unit contents

### SLU01 — Pandas 101

- Create and inspect `Series` and `DataFrame` objects.
- Work with indexes, columns, shapes, values, and data types.
- Summarize data with methods such as `.describe()` and `.info()`.
- Read and write tabular data with functions such as `pd.read_csv()` and methods such as `.to_csv()`.

### SLU02 — Subsetting Data in Pandas

- Select rows and columns with `[]`, `.loc[]`, and `.iloc[]`.
- Build and combine boolean masks to filter data.
- Set, reset, and sort indexes.
- Add and remove rows and columns. With `.drop()`, `axis=0` refers to rows and `axis=1` to columns.

### SLU03 — Visualization with Pandas and Matplotlib

- Use visualization for communication, data understanding, and monitoring.
- Create line, bar, histogram, box, and scatter plots.
- Choose a suitable plot and customize its size, style, labels, legend, title, and annotations.
- Avoid unnecessary or misleading visual elements.

### SLU04 — Basic Statistics with Pandas

- Calculate descriptive statistics, quantiles, ranks, skewness, and kurtosis.
- Inspect distributions with density and cumulative plots.
- Detect outliers and apply simple handling strategies.

### SLU05 — Covariance and Correlation

- Calculate and interpret covariance and correlation.
- Use `.corr()` for Pearson correlation and `.corr(method="spearman")` for Spearman correlation.
- Inspect correlation pairs and the correlation matrix.
- Recognize outliers, spurious correlations, confounding, and the limits of observational data.

### SLU06 — Dealing with Data Problems

- Recognize tidy and untidy data and common numerical-data problems.
- Clean string values, duplicates, invalid entries, missing values, and outliers.
- Apply functions and create missing-value indicators.
- Use appropriate deletion, imputation, and replacement strategies.

### SLU07 — Linear Regression

- Formulate simple and multiple linear-regression problems.
- Understand loss functions, closed-form solutions, and gradient descent.
- Normalize features when required.
- Train, inspect, and use linear-regression models with scikit-learn.

### SLU08 — Metrics for Regression

- Distinguish loss functions from evaluation metrics.
- Use MAE, MSE, RMSE, and R².
- Apply holdout validation and compare training and validation performance.
- Select metrics that match the practical objective and interpret their limitations.

### SLU09 — Logistic Regression

- Formulate binary-classification problems and explore their data.
- Understand the sigmoid function, probabilities, thresholds, odds, and optimization.
- Scale data where appropriate.
- Train models and obtain labels and probabilities with scikit-learn.

### SLU10 — Metrics for Classification

- Understand the limitations of accuracy, particularly with imbalanced classes.
- Use confusion matrices, precision, recall, and F1 score.
- Interpret ROC curves and AUC.

### SLU11 — Tree-Based Models

- Train and interpret decision trees.
- Understand feature selection and feature importance in tree models.
- Compare the advantages and limitations of trees and ensembles.
- Use bagging, random forests, and gradient boosting for classification and regression.

### SLU12 — Feature Engineering

- Prepare numerical and categorical variables.
- Apply suitable transformations, scaling, and categorical encodings.
- Keep training and inference transformations consistent.

### SLU13 — Bias–Variance Trade-off and Model Selection

- Identify underfitting and overfitting through the bias–variance trade-off.
- Use validation and learning curves for model selection.
- Consider memory and computational cost.
- Establish a simple baseline and prevent data leakage.

### SLU14 — Model Complexity and Overfitting

- Select features using correlation, Spearman correlation, mutual information, and model-based methods.
- Use coefficients and tree feature importances appropriately.
- Apply Ridge, Lasso, and Elastic Net regularization.
- Handle class imbalance with appropriate over- and undersampling strategies.

### SLU15 — Hyperparameter Tuning

- Distinguish model parameters from hyperparameters.
- Identify important hyperparameters for the models taught in S01.
- Use grid search and randomized search with appropriate validation.

### SLU16 — Workflow

- Move from data inspection and preparation to training, evaluation, and iteration.
- Start with a suitable baseline and add complexity incrementally.
- Avoid overusing the test set and avoid leakage.
- Use scikit-learn pipelines and compatible custom transformers to keep training and inference consistent.

### SLU17 — Ethics and Fairness

- Consider informed consent, privacy, security, retention, and unintended use.
- Recognize common sources of bias and evaluate model performance across relevant groups.
- Assess fairness across relevant groups.
- Communicate limitations and support auditability, reproducibility, reassessment, and rollback.

### SLU18 — Support Vector Machines (optional)

- Understand margins, linear and nonlinear decision boundaries, soft margins, and kernels.
- Use support-vector classifiers and regressors with scikit-learn.

### SLU19 — k-Nearest Neighbors (optional)

- Understand instance-based learning and the role of distance and neighborhood size.
- Use k-nearest-neighbor classifiers and regressors.
- Recognize the computational and high-dimensional limitations of distance-based methods.

### SLU32 and SLU64 — Hackathon Training (optional)

These two optional units provide additional practice for the hackathon workflow.

## Topics deferred beyond S01

Method chaining, multi-index operations, split–apply–combine, and merging/joining/concatenation are developed in later specializations. Feature unions are introduced with text-classification workflows. Bayesian hyperparameter optimization and detailed multiclass evaluation are outside the current S01 core.
