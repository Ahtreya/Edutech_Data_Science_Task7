# Edutech_Data_Science_Task7
# Data Science Internship - Task 7: Decision Tree Classifier

## Project Overview
This project builds a Decision Tree Classifier using the Scikit-learn library to predict passenger survival on the Titanic dataset. It covers data preprocessing, categorical encoding, feature cleaning, model evaluation, and structural tree visualisation.

## Model Performance
- **Accuracy Score**: 0.754189
- **Precision Score**: 0.702702

## Key Deliverables Included
1. **Source Code**: Python preprocessing, training, and evaluation steps.
2. **Tree Visualization File**: Saved structure plot (`decision_tree_visualization.png`).

---

## Interview Questions & Answers

### 1. What is Gini Impurity?
- **Definition**: Gini Impurity measures how often a randomly chosen element from the set would be incorrectly labeled if it were randomly labelled according to the distribution of labels in the subset.
- **Formula**: $Gini = 1 - \sum (p_i)^2$, where $p_i$ is the probability of an item belonging to class $i$.
- **Interpretation**: A Gini impurity value of `0` implies a perfectly pure node (all items belong to one class). Higher values mean a more even mix of classes. The Decision Tree algorithm selects splits that minimise this impurity.

### 2. Explain pruning in Decision Trees.
- **Definition**: Pruning is a regularisation method used to reduce the size of a fully grown decision tree by removing nodes that add little to no predictive power.
- **Purpose**: It directly combats **overfitting**. A tree with too many branches memorises training noise; pruning ensures it generalises well to unseen data.
- **Approaches**: 
  - **Pre-pruning (Early Stopping)**: Controls structural parameters (like `max_depth` or `min_samples_split`) before training to stop the tree from expanding too much.
  - **Post-pruning**: Allows the tree to grow completely and then trims away insignificant branches from the bottom up based on statistical error costs.
