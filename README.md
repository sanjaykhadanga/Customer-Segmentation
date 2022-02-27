# Customer-Segmentation
**Online-Retail-Customer-Segmentation**
In this project, your task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers

**The need of customer segmentation:**

The differences in customers' behaviour, demographics, geographies, etc. help in classifying them in groups. Learning about different groups in the customer can help with following:

Target Marketing Client understanding Optimal product placement Searching for new customers Revenue growth

**Recency-Frequency-Monetary (RFM) model to determine customer value:**

The RFM model is quite useful model in retail customer segmentation where only the data of customer transaction is available. RFM stands for the three dimensions:

Recency – How recently did the customer purchase? Frequency – How often do they purchase? Monetary Value – How much do they spend? A combination of these three attributes can be defined to assign a quantitative value to customers. e.g. A customer who recently bought high value products and transacts regularly is a high value customer.

**Segmentation with K-means clustering:**

Initially, the data is subject to important stages in an analytics pipeline: exploratory analysis, preprocessing, feature engineering and standardizaton. Then, the unsupervised classification technique, K-means clustering algorithm, is used to determine the ideal segments of customers. Silhouette analysis and related cluster visualizations are leveraged to deduce the optimum value of "K" (number of clusters) in the algorithm. The observations from the results are elaborately discussed before reaching the conclusion from the business perspective.

**what is DBSCAN Clustering:**
Clustering analysis or simply Clustering is 
an unsupervised learning method that 
divides the data points into several
specific batches or groups, such that the 
data points in the same groups have 
similar properties and data points in 
different groups have different properties 
in some sense. It comprises many 
different methods based on differential 
evolution. E.g. K-Means (distance 
between points), Affinity propagation 
(graph distance), Mean-shift (distance 
between points), DBSCAN (distance 
between nearest points), Gaussian 
mixtures (Mahalanobis distance to 
centers), Spectral clustering (graph 
distance), etc
Fundamentally, all clustering methods use 
the same approach i.e. first we calculate 
similarities, and then we use it to cluster 
the data points into groups or batches. 
Here we will focus on Density-based 
spatial clustering of applications with 
noise (DBSCAN) clustering method


**Conclusion**

• K-Means Clustering with Silhouette gives the highest score of 61.9% for number of clusters 3.

• Sales has been increased from 2010 to 2011.

• RFM for Cluster ID box plots tells well about Cluster detail.

• We can deploy this model
