
---

# Exploratory Data Analysis (EDA) and PCA on Iris Dataset

## Overview
This project demonstrates the application of Exploratory Data Analysis (EDA) and Principal Component Analysis (PCA) on the Iris dataset. The Iris dataset is a classic dataset in machine learning, containing data about three species of Iris flowers, with features like sepal length, sepal width, petal length, and petal width.

The steps in this project include:
- Loading and exploring the dataset.
- Performing univariate and multivariate analysis.
- Visualizing distributions, correlations, and outliers.
- Conducting PCA to reduce dimensionality and visualize the data in lower dimensions.

## Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install the required libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Dataset
This project uses the Iris dataset from `sklearn.datasets`. The dataset contains 150 records with 5 features:
- `sepal_length`: Length of the sepal in cm.
- `sepal_width`: Width of the sepal in cm.
- `petal_length`: Length of the petal in cm.
- `petal_width`: Width of the petal in cm.
- `target`: Species of the Iris flower (setosa, versicolor, virginica).

## Steps in the Code

### 1. Load and Explore the Dataset
The Iris dataset is loaded using `load_iris` from `sklearn.datasets` and converted into a pandas DataFrame for ease of manipulation.

### 2. Data Summary
- **First few records** are displayed.
- **Data types** and **missing values** are checked.
- **Statistical summary** of numerical features is shown.

### 3. Univariate Analysis
- **Distribution plots** for each numerical column (sepal length, sepal width, etc.) are created using seaborn's `histplot`.
- **Count plots** for the target variable (`species`) are generated to see the distribution of different flower species.

### 4. Correlation Analysis
- A **correlation heatmap** is created to visualize the relationships between numerical features.

### 5. Pairwise Relationships
- A **pairplot** is created to visualize pairwise relationships between features with different target labels using seaborn.

### 6. Outlier Detection
- **Boxplots** are used to identify potential outliers in the numerical features.

### 7. Principal Component Analysis (PCA)
- The dataset is scaled using `StandardScaler`.
- PCA is applied to reduce the dataset's dimensionality to two components.
- The explained variance ratio of the components is printed.
- A **scatter plot** is created to visualize the dataset in the first two principal components.

## Results
The following insights are provided after executing the analysis:
- Distribution of numerical features.
- Correlation between the features.
- Pairwise relationships across species.
- Detection of outliers in the features.
- Reduced dimensionality using PCA, plotted in a 2D space.

## Conclusion
The EDA and PCA results help in understanding the structure and relationships in the dataset, providing a foundation for further modeling or clustering tasks.

---

