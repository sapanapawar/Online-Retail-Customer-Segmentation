# Online-Retail-Customer-Segmentation:
Using a public online retailer dataset to segment the customers based on purchases and frequency using K-means Clustering.

# Problem Statement:
In this project, the task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

# Attribute Information:

●	InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.

●	StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.

●	Description: Product (item) name. Nominal.

●	Quantity: The quantities of each product (item) per transaction. Numeric.

●	InvoiceDate: Invoice Date and time. Numeric, the day and time when each transaction was generated.

●	UnitPrice: Unit price. Numeric, Product price per unit in sterling.

●	CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.

●	Country: Country name. Nominal, the name of the country where each customer resides.

# Introduction:
The online retail industry has changed the way customers shop as everything is available online. In order to build a loyal customer base, a company needs to deploy various marketing strategies focused on the diverse nature of its customers. 
A possible solution is to segment customers and make targeted marketing strategies for which historical data of customers is required. 
RFM (Recency, Frequency, Monetary) analysis is a technique that helps in extracting insights from the records and can be used for segmentation of customers as well.

# Algorithms:

1.K-Means Clustering:

K-means clustering is one of the simplest and popular unsupervised machine learning algorithms.

The algorithm works as follows:

●	First we initialize k points, called means, randomly.

●	We categorize each item to its closest mean and we update the mean’s coordinates, which are the averages of the items categorized in that mean so far.

●	We repeat the process for a given number of iterations and at the end, we have our clusters.

2. Hierarchical Clustering:

Hierarchical clustering is another unsupervised machine learning algorithm, which is used to group the unlabeled datasets into a cluster and also known as hierarchical cluster analysis or HCA.

In this algorithm, we develop the hierarchy of clusters in the form of a tree, and this tree-shaped structure is known as the dendrogram.

Sometimes the results of K-means clustering and hierarchical clustering may look similar, but they both differ depending on how they work. As there is no requirement to predetermine the number of clusters as we did in the K-Means algorithm.

# Model Performance:
Model can be evaluated by metric such as:

### Silhouette Score:

To study the separation distance between the clusters formed by the algorithm silhouette analysis could be used. The distance between the cluster can be calculated by different types of distance metrics (Euclidean, Manhattan, Minkowski, Hamming). Silhouette score returns the average silhouette coefficient applied on all the samples.

To study the separation distance between the clusters formed by the algorithm silhouette analysis could be used.

For n_clusters=2, the silhouette score is 0.5415858652525395 

For n_clusters=3, the silhouette score is 0.5084896296141937

For n_clusters=4, the silhouette score is 0.48148099614734263

For n_clusters=5, the silhouette score is 0.46501354053484817 

For n_clusters=6, the silhouette score is 0.4169515238218781 

For n_clusters=7, the silhouette score is 0.4150058806779277 

For n_clusters=8, the silhouette score is 0.4072876360981960

# Conclusion:
By observing all the silhouette scores for different values of k, I got the best results for k=3.

So the silhouette score of our best model is 0.50 which can be said to be good for this type of dataset. 








