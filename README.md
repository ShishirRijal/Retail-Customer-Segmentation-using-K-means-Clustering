# Retail Customer Segmentation using K-means Clustering

Welcome to the Retail Customer Segmentation project! This project utilizes a K-means clustering algorithm to group customers of a retail store based on their purchase history. By analyzing customer attributes such as age, annual income, and spending score, the algorithm identifies distinct customer segments, providing valuable insights for marketing and business strategies.

## Table of Contents

- [Libraries Used](#libraries-used)
- [Data Frame](#data-frame)
- [Preprocessing](#preprocessing)
- [Visualization](#visualization)
- [Model Training](#model-training)
- [Evaluation](#evaluation)

## Libraries Used

The following Python libraries are used in this project:

- `pandas`: Data manipulation and analysis library.
- `numpy`: Numerical computing library.
- `seaborn`: Statistical data visualization library.
- `matplotlib`: Data visualization library.
- `sklearn`: Machine learning library for clustering using K-means.
- `os`: Operating system interface for file and directory manipulation.
- `warnings`: Warning control mechanism.
- `plotly`: Interactive plotting library.
- `plotly.express`: High-level interface for plotly to create expressive visualizations.
- `silhouette_score`: Metric for the goodness of a clustering technique.

## Data Frame

The dataset includes the following attributes:

- `CustomerID`: Unique identifier for each customer.
- `Gender`: Gender of the customer (Male/Female).
- `Age`: Age of the customer.
- `Annual Income (k$)`: Annual income of the customer in thousands of dollars.
- `Spending Score (1-100)`: Spending score assigned by the retail store.

```markdown
CustomerID | Gender | Age | Annual Income (k$) | Spending Score (1-100)
-----------|--------|-----|---------------------|-----------------------
    1      |  Male  |  19 |          15         |          39
    2      |  Male  |  21 |          15         |          81
    3      | Female |  20 |          16         |           6
    4      | Female |  23 |          16         |          77
    5      | Female |  31 |          17         |          40
```

## Preprocessing
The data is preprocessed to handle any missing values and ensure its suitability for clustering. Categorical variables are encoded, and the data is scaled for uniformity in feature magnitudes.

## Visualization
Visualizations include bar plots, scatter plots, and an elbow plot. Bar plots are used to visualize gender distribution, while scatter plots highlight the relationships between different attributes. The elbow plot aids in determining the optimal number of clusters for the K-means algorithm.

## Model Training
The K-means clustering algorithm is trained on the preprocessed data using the optimal number of clusters obtained from the elbow plot. The model is then used to assign each customer to a specific cluster.

## Evaluation
The evaluation involves using metrics such as silhouette score and inertia. Silhouette score measures the quality of the clusters, and inertia represents the sum of squared distances from each point to its assigned cluster center. Both metrics are plotted against the number of clusters to identify the optimal configuration.
