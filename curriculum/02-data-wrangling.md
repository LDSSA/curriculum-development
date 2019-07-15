# Data Wrangling Curriculum

## Table of Contents

1. [Curriculum](#1-curriculum)
2. [Topics Not Covered](#2-topics-not-covered)

## 1 Curriculum

| BLU   | Name | Specialization | Status   | Content           |
|-------|------|----------------|----------|-------------------|
| BLU01 | Messy data | Data Wrangling | Proposed | [Content](#blu01) |
| BLU02 | Advanced wrangling  | Data Wrangling | Proposed | [Content](#blu02) |
| BLU03 | Data sources | Data Wrangling | Proposed | [Content](#blu03) |

## Contents

### BLU01

#### Messy data 

##### Main topics

1. Alternative tabular sources 
2. Non-tabular data sources 
3. Common problems and solutions

##### Detailed curriculum
1. Beyond csv 
  - .shuffle 
  - Unusual delimeters (e.g. ";", "|", etc)
  - Corrupt data (e.g. csv files with text boxes over the data) 
  - Non-csv formats 
    - excel (with multiple sheets) 
    - json 
    - encodings
  - Using basic unix to inspect files (`!head` `!tail`, `ls -lh`)
2. Dealing with larger datasets
  - Loading a sample 
  - Loading a random sample (without loading all - explained [here](https://stackoverflow.com/questions/22258491/read-a-small-random-sample-from-a-big-csv-file-into-a-python-data-frame)) 
  - Read csv - chunk size
    - Creating a dataset with the chunks (applying functions to the chunks)   

### BLU02
#### Advanced wrangling (TBD)

##### Main topics

1. group-apply-combine 
  - Vanilla 
  - With lambda functions 
2. Creating tidy datasets 
  - Workflow to get multiple datasets into one 
  - concat, merge
  - inner and outer, left join   
3. Pipelines and Feature Unions 


### BLU03

#### Data sources

##### Main topics

1. SQL 101
- Notes: 
  - Let's try and treat this as _"know it exists & know where to look"_
  - Why SQL is worth knowing, and when it's better to use than Pandas 
  - **KEEP IT SUPER BASIC** in the exercises! 
- Concepts: relational database, tables, foreign & primary key 
- Basic tooling overview 
  - Show alternatives to pandas 
  - Not to be tested in the exercises 
- SELECT *
- COUNT 
- FROM 
- WHERE 
- JOIN
- GROUP BY
- LIMIT 
- AS 
- DISTINCT
- ORDER BY
2. HTML 101 and Beautiful Soup  
  - No change from last year  
3. HTTP requests 
  - GET 
  - Nothing else 

# General notes: 
- When running into content from batch-2 you don't want to erase, leave it as advanced content in an optional separate Learning Notebook 
