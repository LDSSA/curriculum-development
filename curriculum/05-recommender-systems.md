# Recommender Systems Curriculum

## Table of Contents

1. [General](#1-general)
2. [Curriculum](#2-curriculum)
3. [Topics Not Covered](#3-topics-not-covered)


## 1 General
The main changes, in principal, are:
- The content needs to be more practical and applied, based on real-world examples
- Exemplify with public datasets.


## 2 Curriculum

| BLU   | Name | Specialisation | Status   | Content           |
|-------|------|----------------|----------|-------------------|
| BLU10 | Non-Personalised | Recommender Systems | Proposed | [Content](#blu10) |
| BLU11 | Personalised  | Recommender Systems | Proposed | [Content](#blu11) |
| BLU12 | Workflow | Recommender Systems | Proposed | [Content](#blu12) |

## Contents

### BLU10

#### Non-personalised recommender systems

##### Main topics

1. Introduction to recommender systems
2. Ratings matrix, which is a sparse  `scipy` matrix
3. Generic recommender systems.


##### Detailed curriculum

1. Introduction to recommender systems
    1. Intuition
    2. Components of a recommender system 
    3. Taxonomy of recommender systems
    4. ~~Evaluation~~
2. Ratings matrix
    1. Select an open dataset (representative of the hackathon, to avoid surprises)
    2. Intuition about sparsity (i.e., most users don't interact with most items, leading to many empty entires)
    3. Create a ratings matrix as a sparse matrix using `scipy` (pick the type that works best)
3. Generic (or non-personalised) recommender systems, in practice
  1. What are they (with practical examples, in the real-world)
  2. Implement all of these in the selected dataset
    1. Summary statistics
        1. Best-seller
        2. Most popular
        3. Trending (time-decay)
    2. Association rules
        1. You bought X, may be interested in Y
        2. Banana trap (or overwhelming effect)
    3. ~~Evaluate the different generic recommender systems~~.

### BLU11
#### Personalised recommender systems

##### Main topics
1. Collaborative-filtering
2. Content-based filtering
3. Dimensionality reduction.

##### Detailed curriculum
1. Collaborative-filtering
    1. Intuition and real-world use-cases
    2. Cosine distance
        1. For two users or items, `scipy.spatial.distance.cosine`
        2. For all users or items, `sklearn.metrics.pairwise_distances`
    3. Making recommendations
        1. Predicting the rating of an item for an user
    2. Completing the ratings matrix
        1. User-users
        2. Item-item
    3. Top-N recommendations
2. Content-based filtering
    1. Intuition and real-world use-cases
    2. User-tags matrix
    3. Making recommendations
3. Dimensionality reduction
    1. `sklearn.decomposition.PCA`
    2. Making recommendations.
4. When to use what (no sense of progression)

### BLU12

#### Workflow
