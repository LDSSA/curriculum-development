# Time Series Curriculum (W.I.P)



## Table of Contents

1. [General](#1-general)
2. [Curriculum](#2-curriculum)
3. [Topics Not Covered](#3-topics-not-covered)


## 1 General
- The decision to make the Advanced Pandas (multi index) for Time Series optional is to move some of the Time Series concepts to the first BLU, this helps because:
  - This is the time series specialization, so it makes sense that the first BLU talks about time series
  - This makes it possible for the second BLU to completely cover the Classical Models, since the basic concepts have already been introduced.
  - Finally, this makes it possible for the last BLU to focus only on using ML for time series.

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
2. Time Series Concepts
3. Advanced Pandas for Time Series (Optional)  

##### Detailed curriculum
1. Basic Pandas for Time Series
  - Essential functions like pd.to_datetime(), loc[date1:date2], resample
2. Time Series Concepts
  - Time Series decomposition (Trend, Seasonality, Residual)
  - Introduce rolling to get time series trend
  - Introduce shift to get time series lags for seasonality
3. Advanced Pandas for Time Series (Optional)
  - Multi-index, slicing, unstack, etc.


### BLU05
#### Classical Models
  - Here we start using statsmodels

##### Main topics
1. Autocorrelation 
2. ARIMA
3. Exogeneous Variables

##### Detailed curriculum
1. Autocorrelation -> Make connection with pandas diff() for lags. Basically, this automates that search.
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
