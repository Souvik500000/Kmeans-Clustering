### README

#### Project Title: Customer Segmentation

#### Overview
This project involves performing customer segmentation using the Mall Customers dataset. The primary goal is to identify distinct groups of customers based on their purchasing behavior and demographic characteristics, allowing businesses to tailor their marketing strategies more effectively.

#### Files
- **Customer_Segmentation.pdf**: This document contains the analysis performed on the dataset, including data preprocessing, univariate, bivariate, and multivariate analysis, and clustering.
- **Mall_Customers.csv**: The dataset used for this project, which includes the following columns:
  - `CustomerID`: Unique identifier for each customer.
  - `Gender`: Gender of the customer.
  - `Age`: Age of the customer.
  - `Annual Income (k$)`: Annual income of the customer in thousand dollars.
  - `Spending Score (1-100)`: A score assigned to the customer based on their spending behavior.

#### Dependencies
To run the analysis, ensure that the following Python libraries are installed:
- `pandas`
- `seaborn`
- `matplotlib`
- `scikit-learn`

#### Instructions
1. **Data Loading**: Load the `Mall_Customers.csv` dataset using Pandas.
2. **Exploratory Data Analysis**:
   - Perform univariate analysis to explore the distribution of individual features.
   - Conduct bivariate and multivariate analyses to understand the relationships between different variables.
3. **Clustering**:
   - Use the KMeans algorithm to perform customer segmentation.
   - Determine the optimal number of clusters using the elbow method.
   - Analyze the characteristics of each segment and interpret the results.

#### Output
- **Visualizations**: Various plots generated using Seaborn and Matplotlib to illustrate the distribution of data and clustering results.
- **Clusters**: Identification of customer segments based on their annual income and spending score.

#### How to Run
To reproduce the analysis:
1. Open the Jupyter Notebook and run the cells sequentially.
2. Review the visualizations and clustering results to gain insights into customer segments.

---

### Analysis Summary

#### 1. Data Overview
The dataset consists of 200 entries with attributes like `CustomerID`, `Gender`, `Age`, `Annual Income`, and `Spending Score`. The analysis begins by exploring the distribution and relationships between these variables.

#### 2. Univariate Analysis
- **Age**: Customers' ages range from 18 to 70 years, with an average age of approximately 39 years.
- **Annual Income**: The income ranges from 15k to 137k dollars, with an average income of 60.56k dollars.
- **Spending Score**: The score varies between 1 and 99, with a mean of 50.2.

#### 3. Bivariate and Multivariate Analysis
- **Gender Distribution**: 56% of the customers are female, while 44% are male.
- **Age vs. Spending Score**: No strong correlation is observed between age and spending score.
- **Annual Income vs. Spending Score**: The analysis identifies specific clusters of customers based on these two variables.

#### 4. Clustering Analysis
- **KMeans Clustering**:
  - Initially performed clustering on annual income alone, identifying three distinct income-based segments.
  - Further clustering combined annual income with spending score, resulting in more refined customer segments.
- **Elbow Method**: Used to determine the optimal number of clusters, which was found to be three for income-based clustering and a higher number for combined clustering.
- **Cluster Characteristics**: Each cluster was analyzed to understand the average age, income, and spending score of its members.

#### 5. Conclusion
The clustering revealed distinct customer segments, each with unique characteristics. This segmentation can help businesses target their marketing efforts more effectively, focusing on specific customer needs and behaviors.

---

This README and analysis summary should provide a comprehensive overview of the project and guide you through reproducing the results.
