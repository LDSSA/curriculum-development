# Time Series Curriculum (W.I.P)



## Table of Contents

1. [General](#1-general)
2. [Curriculum](#2-curriculum)
3. [Topics Not Covered](#3-topics-not-covered)


## 1 General
The main changes from last years' curriculum are:
- The first BLU will already introduce the time series fundamental concepts, these will be the use cases of the pandas functions. Instead of separating them, like last year.
- The multi index notebook on the fist BLU will be reviewed to see if we can simplify it.
- The second BLU will now cover everything about the classical models and the third BLU everything about the ML-based approach.


## 2 Curriculum

| BLU   | Name | Specialization | Status   | Content           |
|-------|------|----------------|----------|-------------------|
| BLU04 | Time Series Concepts | Time Series | Proposed | [Content](#blu04) |
| BLU05 | Classical Models  | Time Series | Proposed | [Content](#blu05) |
| BLU06 | ML Models | Time Series | Proposed | [Content](#blu06) |

## Contents

### BLU04

#### Time Series Concepts 
  - Here we only use Pandas

##### Main topics

1. Basic Pandas for Time Series
2. Advanced Pandas for Time Series
3. Time Series Concepts


##### Detailed curriculum
1. Basic Pandas for Time Series
  - Essential functions like pd.to_datetime(), loc[date1:date2], resample
2. Advanced Pandas for Time Series
  - Multi-index, slicing, unstack, etc.
3. Time Series Concepts
  - Time Series decomposition (Trend, Seasonality, Residual)
  - Introduce rolling to get time series trend
  - Introduce shift to get time series lags for seasonality



### BLU05
#### Classical Models
  - Here we start using statsmodels

##### Main topics
1. Autocorrelation 
2. ARIMA
3. Exogeneous Variables

##### Detailed curriculum
1. Autocorrelation -> Make connection with pandas shift() for lags. Basically, this automates that search.
  - ACF
  - PACF
  - Stationarity (diff + log)
2. ARIMA
  - Baseline (persistence + rolling mean)
  - AR
  - MA
  - ARIMA
3. Exogenous Variables
  - Introduce causality to distinguish endogenous and exogenous
  - SARIMAX


### BLU06

#### ML Models
  - Make connection that this is not something new. It's simply making use of the time series concepts they've learned to formulate a problem where they can use the ML models they already know.

1. Feature Engineering

2. Regression

3. Classification

3. Time Series Cross-validation

##### Detailed curriculum
1. Feature Engineering
  - Circular Encoding (make connection with scaling for continuous features and categorical encoding for categoricals)
2. Regression 
  - Multi step prediction
3. Classification
4. Time Series Cross-validation
  - Concept Drift

## 3 Topics Not Covered

- Anomaly Detection and Prophet should be refered as additional things to study with reference links
- There are many other classical models such as ES and GARCH that will not be studied but should be mentioned.
- The state of the art for time series is deep learning, which is not covered. 
