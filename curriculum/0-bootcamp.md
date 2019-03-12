Bootcamp
========

1. [Structure](#structure)
2. [Pandas 101](#pandas-101)
3. [Subsetting data](#subsetting-data)

## Structure

| SLU   | Name            | Lead  |
|-------|-----------------|-------|
| SLU01 | Pandas 101      | TBD   |
| SLU02 | Subsetting data | TBD   |

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
