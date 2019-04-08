# Bootcamp Curriculum

## Table of Contents

1. [Curriculum](#1-curriculum)
2. [Topics Not Covered](#2-topics-not-covered)

## 1 Curriculum

| SLU   | Name                                    | Family                 | Status   | Content           |
|-------|-----------------------------------------|------------------------|----------|-------------------|
|       | Notation & Definitions                  | Intro                  | New      |                   |
| SLU01 | Pandas 101                              | Intro                  | To Adapt | [Content](#slu01) |
| SLU02 | Subsetting Data in Pandas               | Intro                  | To Adapt | [Content](#slu02) |
| SLU03 | Visualization with Pandas & Matplotlib  | Intro                  | Existing | [Content](#slu03) |
| SLU04 | Basic Stats with Pandas                 | Basic Practice         | To Adapt | [Content](#slu04) |
| SLU05 | Covariance & Correlation                | Basic Practice         | Existing | [Content](#slu05) |
| SLU06 | Dealing with Data Problems              | Basic Practice         | Existing | [Content](#slu06) |
| SLU07 | Regression with Linear Regression       | Fundamental Algorithms | Existing | [Content](#slu07) |
| SLU08 | Classification with Logistic Regression | Fundamental Algorithms | Existing | [Content](#slu08) |
| SLU09 | Model Validation & Overfitting          | Basic Practice         | Existing | [Content](#slu09) |
| SLU10 | Validation Metrics (Regression)         | Basic Practice         | Existing | [Content](#slu10) |
| SLU11 | Validation Metrics (Classification)     | Basic Practice         | Existing | [Content](#slu11) |
| SLU12 | Support Vector Machines (SVM)           | Fundamental Algorithms | New      | [Content](#slu12) |
| SLU13 | Tree-Based Models                       | Fundamental Algorithms | New      | [Content](#slu13) |
| SLU14 | k-Nearest Neighbors                     | Fundamental Algorithms | New      | [Content](#slu14) |
| SLU15 | Feature Engineering                     | Basic Practice         | Existing | [Content](#slu15) |
| SLU16 | Hyperparameter Tuning                   | Basic Practice         | Existing | [Content](#slu16) |
| SLU17 | Data Sufficiency & Selection            | Basic Practice         | Existing | [Content](#slu17) |
| SLU18 | Ethics & Fairness                       | Basic Practice         | New      | [Content](#slu18) |
| SLU19 | Basic Workflow                          | Basic Practice         | Existing | [Content](#slu19) |

## Contents

### SLU01

#### Pandas 101

##### Main topics

1. Object Creation
2. Basic Functionality
3. Pandas' IO Tools.

##### Detailed curriculum

1. Importing Pandas (i.e., `import pandas as pd`)
2. Object Creation
    1. `pd.Series`
    2. `pd.DataFrame`
3. Basic Functionality
    1. `.head()`, `.tail()`
    2. Attributes
        1. `.shape`
        2. Axis Labels
            1. Series: `.index`
            2. DataFrame: `.index`, `.columns`
        3. Underlying Data
            1. `.values`
            1. `.array`, `to_numpy`
        4. Data Types
            1. Series: `dtype`
            1. DataFrame: `dtypes`
    3. Summarizing Data
        1. `describe`
        2. `info`
4. Pandas' IO Tools
    1. Read a CSV file into a DataFrame
        1. `read_csv`
    2. Store the contents of a DataFrame as a CSV file
        1. `to_csv`
    3. Reference to other similar IO tools to read and write data (e.g., JSON, Excel).

### SLU02

#### Subsetting Data in Pandas

##### Main topics

1. Basic Indexing
2. Adding Rows & Columns
3. Removing Rows & Columns

##### Detailed curriculum

1. Basic Indexing
    1. Set the DataFrame index
        1. Using `index=` on object creation with `pd.Series` or `pd.DataFrame`
        2. Using `index_col=` when reading with `pd.read_csv`
        3. Using existing columns
            1. `reset_index()`
            2. `set_index()`, `sort_index()`
    2. Indexers: `[]`, `.loc[]`, and `.iloc[]`
        1. Selecting Rows with `.loc[]` and `.iloc[]`
            1. Selection by Label, i.e., `.loc[indexer]`
                1. Single row by passing a single Label
                2. Multiple rows
                    1. By passing a list or array of labels
                    2. A slice object, i.e., slice notation
                    3. A boolean array or Series
            2. Selection by Position, i.e., `.iloc[position]`
                1. Single row by passing an integer
                2. Multiple rows
                    1. By passing a list or array of integers
                    2. A slice object with integers
                    3. A boolean array
        2. Selecting Columns with `[]`
            1. Using the indexing operator `[]`, i.e., square brackets notation `df[col]`
                1. Single column
                2. Multiple columns
                    1. By passing a list or array of columns, in any order
            2. Attribute access (not indexing), i.e., dot notation  `df.col`
        3. Multi-Axis Indexing with `.loc[]` and `.iloc[]`
            1. Multi-Axis Selection by Label
                1. `.loc[row_indexer, col_indexer]`
            2. Multi-Axis Selection by Position
                1. `.iloc[row_position, col_position]`
2. Adding Rows & Columns
    1. Using the indexing operator `df[new_col]=`
    2. Assigning new columns to a DataFrame with `.assign()`
3. Removing Rows & Columns
    1. Using `drop()` to remove specified labels
        1. From Rows
            1. `.drop(axis=1)`, `.drop(columns=)`
        2. From Columns
            1. `drop()`

---

### SLU03

#### Visualization with Pandas & Matplotlib

##### Main topics

1. Basic Plotting in Pandas
2. Different Types of Plots
3. Formatting & Styling

##### Detailed curriculum

1. Importing Matplotlib
    1. `import matplotlib.pyplot as plt`
    2. `%matplotlib inline`
2. Basic Plotting in Pandas
    1. Line plots
        1. Series: `.plot()`
        2. DataFrame: `.plot()`, `.plot(x=, y=)`
3. Different Types of Plots
    1. How to choose the right type
    2. Bar plots
        1. Using `.plot(kind='bar')`, `.plot(kind='barh')`
        2. Using `.plot.bar()`, `.plot.barh()`
        3. Stacked bar plots with `stacked=True`
    3. Histograms
        1. Using `.plot(kind='hist')`
        2. Using `.plot.hist()`, `.plot.hist(xlim=)`
    4. Boxplot
        1. Using `.plot(kind='box')`
        2. Using `.plot.box()`, `.plot.box(vert=False)`
    5. Scatterplot
        1. Using `.plot(kind='scatter')`
        2. Using `.plot.scatter()`
4. Formatting & Styling
    1. Using the Matplotlib API (some can be used on Pandas directly)
        1. Size: `matplotlib.rcParams["figure.figsize"]`
        2. Styles: `plt.style.use()`
        3. Legend: `.plot(legend=)`, `plt.legend()`
        4. Labels: `plt.xlabel()`, `plt.ylabel()`
        5. Title: `plt.title()`
        6. Text: `plt.figtext()`
    2. Avoiding chartjunk
        1. Don't use unnecessary and/or confusing elements
        2. Use the minimum set of visuals necessary to be informative.

---

### SLU04

#### Basic Stats with Pandas

##### Main topics

1. Descriptive Statistics
2. Inspecting Distributions
3. TBD

##### Detailed curriculum

1. Descriptive Statistics in Pandas
    1. `.count()`
    2. `.sum()`, `.cumsum()`
    3. `.nunique()`
    4. `.mean()`, `.median()`
    5. `.mode()`
    6. `.min()`, `.max()`
    7. `.idxmin()`, `.idxmax()`
    8. `.var()`, `.std()`
    9. `.quantile()`
2. Inspecting Distributions
    1. Skew with `.skew()`, plus interpretation
    2. Kurtosis with `.kurt()`, plus interpretation
    3. Probability Density Function (PDF)
        1. Using `.plot(kind='density')`
        2. Using `.plot.density()`
    4. Cumulative Density Function (CDF)
        1. Using `.plot(kind='hist', histtype='step', density=True, bins=100, cumulative=True)`

---

### SLU05

#### Covariance & Correlation

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU06

#### Dealing with Data Problems

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU07

#### Regression with Linear Regression

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU08

#### Classification with Logistic Regression

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU09

#### Model Validation & Overfitting

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU10

#### Validation Metrics

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU11

#### Validation Metrics (Classification)

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU12

#### Support Vector Machines (SVM)

##### Main topics

1. What is it
2. When to use it
3. How to use it

##### Detailed curriculum

TBD.

---

### SLU13

#### Tree-Based Models 

##### Main topics

1. What is it
2. When to use it
3. How to use it

##### Detailed curriculum

TBD.

---

### SLU14

#### k-Nearest Neighbors

##### Main topics

1. What is it
2. When to use it
3. How to use it

##### Detailed curriculum

TBD.

---

### SLU15

#### Feature Engineering

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU16

#### Hyperparameter Tuning

##### Main topics

1. TBD
2. TBD
3. TBD

#### Detailed curriculum

TBD.

---

### SLU17

#### Data Sufficiency & Selection

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU18

#### Ethics & Fairness

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

---

### SLU19

#### Basic Workflow

##### Main topics

1. TBD
2. TBD
3. TBD

##### Detailed curriculum

TBD.

## 2 Topics Not Covered

1. Pandas
    1. `.drop_duplicates()`
    2. `.select_dtypes()`
    3. `.pop()`
    4. Method chaining
    5. Multi-Index and Advanced Indexing
    6. Merging, joining, and concatenating
    7. Split-apply-combine