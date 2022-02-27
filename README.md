# Customer-Segmentation
**Online-Retail-Customer-Segmentation**
In this project, your task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers

**The need of customer segmentation:**

The differences in customers' behaviour, demographics, geographies, etc. help in classifying them in groups. Learning about different groups in the customer can help with following:

Target Marketing Client understanding Optimal product placement Searching for new customers Revenue growth

**Data Overview:

Data: This is a transnational data set that
contains all the transactions occurring 
between 01/12/2010 and 09/12/2011 for 
a UK-based and registered non-store 
online retail. The company mainly sells 
unique all-occasion gifts. Many customers 
of the company are wholesalers.

**Data Attributes

1. InvoiceNo: Invoice number. Nominal, a 
6-digit integral number uniquely assigned 
to each transaction. If this code starts with 
the letter ‘ca, it indicates a cancellation.

2. StockCode: Product (item) code. 
Nominal, a 5-digit integral number 
uniquely assigned to each distinct 
product.

3. Description: Product (item) name. 
Nominal.

4. Quantity: The quantities of each 
product (item) per transaction. Numeric.

5. InvoiceDate: Invoice Date and time. 
Numeric, the day and time when each 
transaction was generated.

6. UnitPrice: Unit price. Numeric, Product 
price per unit in sterling.

7. CustomerID: Customer number. 
Nominal, a 5-digit integral number 
uniquely assigned to each customer.

8. Country: Country name. Nominal, the 
name of the country where each 
customer resides.

Data Snapshot:

![image](https://user-images.githubusercontent.com/89900907/155872653-bf532f0e-d0b3-4505-8d4b-68e377edc14f.png)

**Implementation:**

**Exploring the Data:

Data was processed and cleaned. Here the 
duplicates were removed and the missing 
values were handled.

**Country:

Since the data, taken from the UCI 
Machine Learning repository describes the 
data based on transactions for a UK-based 
and registered non-store online retail, let 
us check the percentage of orders from 
each country in the data.

**Customers and Products:

The total number of products, 
transactions and customers in the data, 
which correspond to the total unique 
stock codes was found out
It can be seen that the data concern 4372 
users and that they bought 3958 different 
products. The total number of 
transactions carried out is of the order of 
∼ 24000.
Many Orders were canceled and across 
the countries. As per the data, if the 
invoice number code starts with the letter 
‘C’, it indicates a canceled order.

**Stock Code:

several types of peculiar transactions, 
connected i.e., port charges, bank fees, 
discounts, gifts, Carry bags, Samples, 
Amazon fees, transaction fees which
needed to be analyzed.

**Cohort Analysis

Time cohorts: It groups customers 
by their purchase behavior over 
time.

Behavior cohorts: It groups 
customers by the product or 
service they signed up for.

Size cohorts: Refer to various sizes 
of customers who purchase the 
company's products or services. 
This categorization can be based
on the amount of spending in 
some period

**Recency-Frequency-Monetary (RFM) model to determine customer value:**

The RFM model is quite useful model in retail customer segmentation where only the data of customer transaction is available. RFM stands for the three dimensions:

Recency – How recently did the customer purchase? Frequency – How often do they purchase? Monetary Value – How much do they spend? A combination of these three attributes can be defined to assign a quantitative value to customers. e.g. A customer who recently bought high value products and transacts regularly is a high value customer.

**Segmentation with K-means clustering:**

Initially, the data is subject to important stages in an analytics pipeline: exploratory analysis, preprocessing, feature engineering and standardizaton. Then, the unsupervised classification technique, K-means clustering algorithm, is used to determine the ideal segments of customers. Silhouette analysis and related cluster visualizations are leveraged to deduce the optimum value of "K" (number of clusters) in the algorithm. The observations from the results are elaborately discussed before reaching the conclusion from the business perspective.

**RFM analysis:**
From the above analysis, we can see that 
there should be 4 clusters in our data. To 
understand what these 4 clusters mean in 
a business scenario, we should look back 
at the table comparing the clustering 
performance of the RFM Segmentation 
Model and 4 clusters for the mean values 
of recency, frequency, and monetary 
metric. On this basis, let us label the 
clusters as ‘New customers’, ‘Lost 
customers’, ‘Loyal customers’, and ‘At 
Risk customers’.

![image](https://user-images.githubusercontent.com/89900907/155872566-f29a274d-d1de-4f10-a90a-17ebb04bf82d.png)

**Calculation of Silhouette score**

Silhouette score is used to evaluate the 
quality of clusters created using clustering 
algorithms such as K-Means in terms of 
how well samples are clustered with other 
samples that are similar to each other. 
The Silhouette score is calculated for each 
sample of different clusters. To calculate 
the Silhouette score for each 
observation/data point, the following 
distances need to be found out for each 
observation belonging to all the clusters:

**Applying elbow method:**

Elbow is one of the most famous methods 
by which you can select the right value of 
k and boost your model performance. We 
also perform hyperparameter tuning to 
choose the best value of k. Let us see how 
this elbow method works. It is an 
empirical method to find out the best 
value of k. it picks up the range of values 
and takes the best among them. It 
calculates the sum of the square of the 
 
points and calculates the average 
distance.
When the value of k is 1, the withincluster sum of the square will be high. As 
the value of k increases, the within-cluster 
sum of the square value will decrease.
Finally, we will plot a graph between kvalues and the within-cluster sum of the 
square to get the k value. we will examine 
the graph carefully. At some point, our 
graph will decrease abruptly. That point 
will be considered as a value of k.

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
