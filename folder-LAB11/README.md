## Questions & Answers

### 1. Why is this an unsupervised learning problem?
Because the dataset does not contain labeled outputs, and the model discovers customer groups automatically.

### 2. Why did we remove the CUST_ID column?
Because it is only an identification column and does not describe customer behavior.

### 3. Which columns had missing values?
The missing values were found in:
- CREDIT_LIMIT
- MINIMUM_PAYMENTS

### 4. How did you handle the missing values?
Missing values were filled using the mean value of each column.

### 5. Why is scaling important before applying K-Means?
Because K-Means depends on distance calculations, and scaling prevents large-value features from dominating the clustering process.

### 6. Which K value did you choose?
We chose K = 3 based on the elbow curve and silhouette scores because it provided a good balance between clustering quality and simplicity.

### 7. Describe each customer segment.
- Cluster 0: Customers with high balances and heavy cash advance usage.
- Cluster 1: High-value customers with high purchases and frequent card usage.
- Cluster 2: Low-activity customers with lower balances and purchases.

### 8. Which cluster represents high-value customers?
Cluster 1 represents high-value customers because it has the highest purchases, payments, and credit limits.

### 9. Which cluster relies more on cash advance?
Cluster 0 relies more on cash advance because it has the highest cash advance values and transactions.

### 10. How can companies use these clusters?
Companies can create targeted marketing strategies for each customer segment, such as loyalty rewards for high-value customers and promotional offers for low-activity customers.
