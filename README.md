## Mall Customer Segmentation

### Project Overview

This project focuses on **segmenting mall customers** into distinct groups based on their demographic and behavioral data. Using unsupervised machine learning techniques, specifically **K-Means clustering**, the goal is to identify hidden patterns and create customer segments. This is a fundamental task in marketing and business strategy, as it allows for targeted campaigns and personalized customer experiences.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Customer Segmentation Tutorial in Python](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
  * **Size**: 200 entries, 5 columns
  * **Key Features**:
      * `Gender`, `Age`, `Annual Income (k$)`, `Spending Score (1-100)`. The `CustomerID` column is dropped as it is a unique identifier.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates.
      * **Exploratory Data Analysis**: Histograms and boxplots were used to visualize the distribution of numerical features. A heatmap was generated to show the correlation between these features.
      * **Label Encoding**: Applied to the `Gender` column to convert it into a numerical format.
      * **Unsupervised Learning**: The **K-Means clustering algorithm** was used for segmentation. The optimal number of clusters was determined using the **Elbow Method** by plotting the inertia for a range of clusters.
      * **Segmentation Scenarios**: The model was applied to three different feature combinations to explore various customer segments:
        1.  **Age and Spending Score**: Identified 4 distinct clusters.
        2.  **Annual Income and Spending Score**: Identified 5 distinct clusters, which is a classic and highly interpretable segmentation for marketing.
        3.  **Age, Annual Income, and Spending Score**: Identified 6 clusters in a 3D space, showing more nuanced segmentation.
  * **Key Findings**:
      * The segmentation based on **Annual Income and Spending Score** is particularly insightful for creating marketing personas, revealing groups like "high-income, high-spending" and "low-income, low-spending" customers.
      * The visualizations clearly show the distinct clusters formed by the algorithm.

-----

### Purpose and Applications

  * **Targeted Marketing**: Enables businesses to design specific marketing campaigns for each customer segment, increasing their effectiveness.
  * **Personalized Experiences**: Helps in tailoring product recommendations, offers, and services to different customer groups.
  * **Business Strategy**: Provides a data-driven approach to understand the customer base and inform business strategy.
  * **Retail Management**: Assists in optimizing store layouts, product assortments, and promotions for different customer segments.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Mall-Customer-Segmentation-Using-Kmeans.git
cd Mall-Customer-Segmentation-Using-Kmeans
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Exploring other clustering algorithms like DBSCAN or Hierarchical Clustering to see if they produce different or more meaningful segments.
  * Performing a more in-depth analysis of each cluster to describe the characteristics of the customer segments in detail.
  * Investigating the impact of scaling on the clustering results, especially when using features with different units and scales.
  * Adding a pipeline for new customer data to be automatically classified into one of the existing segments.
