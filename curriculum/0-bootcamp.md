Bootcamp
========

| SLU   | Name                                      | Lead  |
|-------|-------------------------------------------|-------|
| SLU01 | [Pandas 101](#pandas-101)                 | TBD   |
| SLU02 | [Subsetting data](#subsetting-data)       | TBD   |
| SLU03 | [Transforming Data](#transforming-data)   | TBD   |
| SLU04 | [Data Visualization](#data-visualization) | TBD   |
| SLU05 | [Basic Stats](#basic-stats)               | TBD   |
| SLU06 | [Intermediate Stats](#intermediate-stats) | TBD   |
| SLU07 | [Advanced Stats](#advanced-stats)         | TBD   |

## Pandas 101

1. Help commands on Jupyter **--> NEW <--**
    1. Using tab for autocomplete
    2. `?`
    3. `??`
2. What is Pandas
3. Importing Pandas (i.e., `import pandas as pd`)
4. Intro to Data Structures
5. `pd.Series`
    1. From `list`
        1. Using `index=`
    2. From `dict`
6. ~~`dtypes`~~ **removed**
7. `pd.Series.values`
8. `pd.Series.index`
9. `pd.DataFrame`
    1. From `list`
      1. Using `columns=`
      1. Using `index=`
    2. From `dict`
      1. Of `list`
      2. Of `pd.Series`
    3. Adding new columns
      1. `df[new_col]=`
      2. `df.assign(new_col=)` **--> NEW <--**
10. `pd.DataFrame.index`
11. `pd.DataFrame.columns`
12. `pd.DataFrame.head`
13. `pd.DataFrame.tail`
14. `pd.DataFrame.count`
15. `pd.DataFrame.info`
16. `pd.DataFrame.describe`
17. `pd.DataFrame.shape`
18. `pd.read_csv`

## Subsetting Data

1. `pd.options.display.max_rows`
2. `index_col` in `pd.read_csv`
3. Selecting columns
    1. Dot notation `df.col`
    2. Brackets notation `df[col]`
        1. Selecting multiple columns
4. Selecting rows
    1. Selecting by position with `iloc`
    2. Select by index name with `loc`
5. Multi-axis indexing with `.loc`
    1. Comparison with chain indexing
6. Masks
    1. `pd.DataFrame.mask`
    2. `pd.DataFrame.where`
7. Subsetting data on conditions
    1. One condition
    2. Not operator `~`
    3. Combining conditions with `&`, `|`
8. Data types
    1. `dtypes`
    2. `select_dtypes`
9. `nlargest`
10. `nsmallest`

## Transforming Data

1. `pd.DataFrame.drop(labels=)`
2. `pd.DataFrame.drop(columns=)`
3. `pd.DataFrame.drop(inplace=)`
4. `pd.DataFrame.copy`
5. Mathematical operations
6. `pd.DataFrame.groupby`
7. `GroupBy.groups`
8. `GroupBy.size`
9. `GroupBy.agg`
10. `pd.concat`
11. `pd.DataFrame.sort_index`
12. `pd.DataFrame.reset_index`
13. `pd.DataFrame.set_index`
14. `pd.DataFrame.sort_values`

## Data Visualization

1. `pd.DataFrame.hist`
2. `pd.DataFrame.boxplot`
3. `pd.DataFrame.plot`
4. `pd.DataFrame.plot(kind=)`
4. `pd.DataFrame.plot.scatter`
5. `pd.DataFrame.plot.barh`
6. `plt.style.available`
7. `plt.style.use`
8. `plt.legend`
9. `plt.title`
10. `plt.ylim`
11. `plt.xlabel`
12. `plt.ylabel`
13. `plt.figtext`

## Basic Stats

1. ~~Numpy~~
2. `utils`
3. `pd.Series.mode`
4. `pd.Series.mean`
5. `pd.Series.median`
6. `pd.Series.var`
7. `pd.Series.std`
8. `pd.Series.quantile`
9. `pd.crosstab`
10. `pd.crosstab(margins=True)`
11. `pd.Series.unique`
12. `pd.Series.max`
13. `pd.Series.idxmax`
14. `pd.Series.min`
15. `pd.Series.idxmin`

## Intermediate Stats

1. Covariance
2. `pd.Series.cov`
3. Correlation
4. `pd.Series.corr`
5. Pearson correlation
6. Spearman correlation
7. `pd.DataFrame.rank`
8. `pd.Series.corr(method=)`
9. Correlation matrix
10. `seaborn`
11. `sns.heatmap`
12. Spurious correlations
13. Observation data
14. Experimental data
15. Confounding variables

## Advanced Stats

1. `numpy`
2. `scipy.stats`
3. Normal distribution
4. `stats.norm.rvs`
6. `stats.norm.cdf`
8. `stats.norm.ppf`
9. `stats.norm.pdf`
10. Binomial distribution
4. `stats.binom.rvs`
6. `stats.binom.cdf`
8. `stats.binom.ppf`
9. `stats.binom.pdf`
10. Geometric distribution
11. Exponential distribution
12. Poisson distribution
13. Sample mean
14. `.sample()`
15. `np.random.seed`
16. `np.random.choice`
17. Confidence intervals
18. Hypothesis testing
20. `stats.ttest_1samp`
21. `stats.chisquare`
