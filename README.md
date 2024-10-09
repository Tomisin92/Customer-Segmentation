# Mall Customer Segmentation using K means clustering
## Objective
The primary goal of this analysis is to identify unique customer segments by examining demographic and behavioral data. With segmentation, the mall can improve customer satisfaction, tailor marketing messages to each customer type, and maximize the effectiveness of marketing resources.

## key attributes:
Customer ID: Unique identifier
Genre: Gender (Male or Female)
Age: Ranging from 18 to 70 years, with a mean of approximately 38.85 years.
Annual Income: Ranging from $15k to $137k, with a mean of $60.56k.
Spending Score: A behavioral score from 1 to 100 based on customer purchasing power and habits, with an average of 50.2.

## Key Descriptive Statistics:
Age: The data shows moderate variability with a standard deviation of 13.97, suggesting that customers span a wide age range, although most are clustered around middle age.
Annual Income: With a standard deviation of 26.26, there is significant income diversity, ranging widely from low-income to high-income customers.
Spending Score: The score has a standard deviation of 25.82, indicating diverse spending behavior across the customer base, with scores distributed across low, medium, and high ranges.

## Gender Distribution
The dataset includes 112 female customers and 88 male customers. This distribution provides a gender balance suitable for analysis but indicates a slight majority of female customers.

## Clustering Analysis Using K-Means
The K-Means algorithm was applied to segment customers based on their Annual Income and Spending Score. The steps included:

Within-Cluster Sum of Squares (WCSS): To determine the optimal number of clusters, the WCSS metric was used, plotted against the number of clusters (k) in an Elbow Curve.

Optimal Clusters: The elbow curve suggested that 5 clusters best fit the data, minimizing intra-cluster variance while avoiding over-segmentation.
Cluster Descriptions:

Cluster 1 (Miser): Customers with both low annual income and low spending score. This group represents low-value customers who likely spend only on essential purchases.
Cluster 2 (General): Customers with moderate income and spending score, falling into an average spending range. This is a sizable customer group that represents standard, reliable revenue for the mall.
Cluster 3 (Target): High spending scores irrespective of income levels, indicating a preference for quality or convenience.
Cluster 4 (Spendthrift): High-income customers with high spending scores, marking them as the most valuable group for premium and high-margin products.
Cluster 5 (Careful): Moderate income but relatively lower spending scores, suggesting budget-conscious behavior despite average earnings.

## Statistical Insights from Clustering
1. Intra-Cluster Variability: Each cluster has distinct statistical characteristics that provide insights into spending patterns relative to income:

Cluster 4 (Spendthrift) shows the highest income and spending variance, indicating that spending capacity grows with income among these customers.
Cluster 1 (Miser) has low variance in both income and spending, suggesting a uniform approach to minimal spending within this group.
2. Cluster Sizes:

Distribution: Clusters vary in size, with the "General" group being the largest. This suggests that most customers fall into a moderate-income, moderate-spending range, ideal for regular promotions and discounts to increase engagement.
Outlier Segment (Spendthrift): Though smaller in size, this cluster holds significant value due to high spending capacity. Targeting these customers with premium offerings could maximize revenue.

## Correlation Analysis
Correlation Between Variables:

Age and Spending Score: No significant correlation was observed, implying that spending habits do not directly correlate with age.
Income and Spending Score: A moderate positive correlation was found, indicating that higher income levels moderately influence higher spending behavior.
Income and Age: A weak positive correlation suggests that income increases slightly with age, although age is not a strong predictor of income in this dataset.

## Cluster Visualization and Patterns-lbow Method:

The plot of WCSS values across clusters shows a clear "elbow" at 5 clusters, justifying this choice as it minimizes within-cluster variance while avoiding unnecessary complexity.
Spending Patterns by Cluster:

Low-Spending Clusters (Clusters 1 and 5) display spending scores mostly below the median (50), suggesting cost-conscious behavior that can be targeted with discount-driven promotions.
High-Spending Cluster (Cluster 4) shows spending scores above 75, making it ideal for premium, exclusive offerings.

## Conclusion and Actionable Insights
The quantitative analysis suggests diverse spending behaviors and income levels across clusters, each providing unique insights for customer engagement strategies.
Low-Income, Low-Spending Segments: Engage with discounts and value deals to increase footfall among these groups.
High-Income, High-Spending Segments: Target with premium products and exclusive services to maximize revenue from this high-value cluster.
Moderate-Income, Moderate-Spending Segments: Standard promotional campaigns and loyalty programs could strengthen engagement and encourage incremental spending.
