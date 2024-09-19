# LAB-Unsupervised-Learning-Dimensionality-Reduction

## Introduction

Dimensionality reduction is a key technique in unsupervised learning that helps simplify models, reduce computational cost, and visualize data effectively. In this lab, we will explore Principal Component Analysis (PCA) and t-Distributed Stochastic Neighbor Embedding (t-SNE) techniques to reduce the dimensions of a high-dimensional dataset and gain insights from it.

## Setup Instructions

Follow the steps below to set up the environment and reproduce the results from this lab:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/codeskills-ai/LAB-Unsupervised-Learning-Dimensionality-Reduction.git
    cd LAB-Unsupervised-Learning-Dimensionality-Reduction
    ```

2. **Create a virtual environment and install the required packages**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Start Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```

## Iteration 1: Introduction to Dimensionality Reduction (Wine Dataset with PCA)

Make sure to import the necessary libraries like `numpy`, `pandas`, `matplotlib`, `seaborn`, and `sklearn`.

1. **Load the Wine Dataset**:
   - Load the Wine dataset directly from `sklearn` and convert it into a Pandas DataFrame for better handling.

2. **Data Exploration**:
   - Calculate descriptive statistics for each column.
   - Observe the distribution of the target variable `quality` and visualize the correlation between features using a heatmap.

3. **Discussion**:
   - Which features seem to be most correlated with the target variable `quality`?
   - Are there any features that appear irrelevant or redundant?

## Iteration 2: Principal Component Analysis (PCA) on Wine Dataset

1. **Preprocessing**:
   - Standardize the features using `StandardScaler` so that all features are on the same scale.

2. **Applying PCA**:
   - Apply PCA to reduce the dataset to 2 principal components.
   - Visualize the cumulative explained variance and plot the first two principal components.

3. **2D Visualization**:
   - Create a 2D scatter plot of the first two principal components. Use different colors for each `quality` value to observe patterns.

4. **Discussion**:
   - Can you observe any clear separation between different quality values?
   - How much variance is explained by the first two principal components?

## Iteration 3: t-Distributed Stochastic Neighbor Embedding (t-SNE) on Digits Dataset

1. **Load the Digits Dataset**:
   - Load the Digits dataset from `sklearn` and convert it into a Pandas DataFrame.

2. **Preprocessing**:
   - Standardize the features using `StandardScaler` so that all features are on the same scale.

3. **Applying t-SNE**:
   - Use t-SNE to reduce the dataset to 2 components. Adjust `perplexity` and other parameters as needed.

4. **2D Visualization**:
   - Create a scatter plot of the two t-SNE components, using different colors for each `digit` value.

## Iteration 4: Evaluation and Conclusions

**Evaluation of Techniques**:
   - Compare the effectiveness of PCA and t-SNE using a simple classifier like KNN and evaluate accuracy before and after applying each technique.
   - Train a KNN classifier on both PCA-reduced and t-SNE-reduced datasets and compare the performance with the original dataset.

## Bonus:

- **Try with a Different Dataset**: Implement the above steps using another dataset available in `sklearn`, such as the Iris dataset for PCA and Fashion MNIST for t-SNE, and compare the results obtained.

