
<h1>Customer Segmentation Using K-Means Clustering</h1>

<h2>Overview</h2>
<p>
    Customer segmentation is a powerful tool for businesses to understand their customers better and tailor marketing strategies accordingly. This project leverages K-Means clustering, a popular unsupervised machine learning algorithm, to segment customers based on their purchasing behaviors and relevant attributes. By identifying distinct customer groups, the project aims to provide insights that can help in optimizing marketing efforts and improving overall business performance.
</p>

<h2>Objectives</h2>
<ul>
    <li><strong>Customer Segmentation:</strong> To categorize customers into distinct groups based on their purchasing behaviors, demographics, and product preferences.</li>
    <li><strong>Insights and Analysis:</strong> To gain actionable insights into the characteristics of different customer segments, enabling more targeted marketing and data-driven decision-making.</li>
</ul>

<h2>Data Preparation</h2>
<ol>
    <li><strong>Loading Data:</strong> The dataset is loaded from a CSV file containing various customer and order-related attributes.</li>
    <li><strong>Feature Selection:</strong> Key features relevant to clustering are retained, such as customer recency, quantity purchased, total sales, discount, and profit. Unnecessary columns are removed.</li>
    <li><strong>Feature Engineering:</strong> New features are created to enhance analysis. For example, 'Total Sales' is calculated by multiplying 'Quantity' with 'Sales,' and 'Recency' is computed as the number of days since the customer's last purchase.</li>
</ol>

<h2>Feature Scaling</h2>
<p>
    Before applying the K-Means clustering algorithm, features are standardized to ensure they are on a similar scale. This step is crucial as K-Means is sensitive to the scale of the data, and standardization helps in achieving more accurate clustering results.
</p>

<h2>Determining the Number of Clusters</h2>
<p>
    The optimal number of clusters is determined using the <strong>Elbow Method</strong>. This involves plotting the inertia (sum of squared distances of samples to their nearest cluster center) for different numbers of clusters and identifying the 'elbow' point, where the rate of decrease sharply slows down. This point indicates the most appropriate number of clusters.
</p>

<h2>Applying K-Means Clustering</h2>
<p>
    After determining the optimal number of clusters, K-Means clustering is applied to the dataset. The algorithm groups customers into clusters based on the similarity of their features. Each customer is assigned a cluster label, and cluster centers are computed to represent the central tendencies of each segment.
</p>

<h2>Analysis and Visualization</h2>
<p>
    The characteristics of each cluster are analyzed by aggregating and summarizing the features within each segment. Visualization tools, such as pair plots and cluster plots, are employed to help interpret the clusters and their distinguishing attributes. This analysis provides a clear understanding of the different customer segments.
</p>

<h2>Evaluating Clustering Performance</h2>
<p>
    The quality of the clustering results is evaluated using the <strong>Silhouette Score</strong>, which measures how similar a customer is to their own cluster compared to other clusters. A higher silhouette score indicates that the clusters are well-defined and distinct.
</p>

<h2>Saving and Reporting Results</h2>
<p>
    The final segmented data, including cluster labels, is saved to a CSV file for further analysis and reporting. Additionally, the cluster centers are exported to better understand the typical characteristics of each customer segment.
</p>

<h2>Conclusion</h2>
<p>
    This project successfully segments customers into distinct groups using K-Means clustering, providing valuable insights into customer behaviors and preferences. These insights can be used to tailor marketing strategies, improve customer engagement, and make more informed business decisions. The structured approach taken in this project ensures that the clustering results are robust, interpretable, and actionable.
</p>

<h2>Files in This Repository</h2>
<ul>
    <li><strong>data/:</strong> Contains the original dataset and the processed dataset with cluster labels.</li>
    <li><strong>notebooks/:</strong> Jupyter notebooks with code for data preparation, clustering, analysis, and visualization.</li>
    <li><strong>reports/:</strong> Contains reports and visualizations generated from the analysis.</li>
    <li><strong>README.md:</strong> This file, providing an overview of the project.</li>
</ul>

<h2>How to Run</h2>
<ol>
    <li>Clone this repository.</li>
    <li>Install the necessary dependencies from <code>requirements.txt</code>.</li>
    <li>Run the Jupyter notebooks in the <code>notebooks/</code> directory to see the data preparation, clustering, and analysis steps.</li>
    <li>The final segmented data can be found in the <code>data/</code> directory.</li>
</ol>

<h2>Dependencies</h2>
<ul>
    <li>Python 3.x</li>
    <li>pandas</li>
    <li>numpy</li>
    <li>scikit-learn</li>
    <li>matplotlib</li>
    <li>seaborn</li>
</ul>

<p>To install the required packages, you can use the following command:</p>

<pre><code>pip install -r requirements.txt</code></pre>

</body>
</html>
