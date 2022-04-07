# High-Value Customer Identification.

<img src="https://y26uq11r8xr1zyp0d3inciqv-wpengine.netdna-ssl.com/wp-content/uploads/2020/01/197-1.jpg" alt="drawing" width="70%"/>

## 1.0. Description: 

This project aims to realize a selection of high value customers for a British E-Commerce company using Clustering techniques.

## 2.0. Business Problem:

It is known that exists several types of customers in an E-Commerce Company, with different types of behavior. It is also known that different types of behavior requires different types of approach by the business team. So, the context of the problem it's a british E-Commerce company whose Marketing Team wants to build a Loyalty Program after realizing that some customers of their purchase base buy more expensive products, with hight frequency, and end up contributing with a significant share to the companie's revenue.

The challenge is to realize a selection of eligible customers for the program, utilizing advanced Data Science techniques.

## 3.0. Solution Strategy:

### 3.1. Data Collection:

Download of the CSV file from the Kaggle Competition.

### 3.2. Data Description:

Here I focused on seeing the quantitity and quality of the data. Aimed to answer questions like how much data is available and the conditition of them. Checked the columns name, data dimensions, data types, NA's and done a descriptive statistics with all features, including numerical and categorical.

### 3.3. Data Filtering:

Filtered data considering descriptive statistics and business assumptions.

### 3.4. Feature Engineering: 

Derivated new features that make business sense from the existing ones and could pontentially help on the Clustering Models.

### 3.5. Exploratory Data Analysis: 

Sought to understand a litte bit more of the data with Pandas Profiling, pairplot and Space Study.

#### **3.5.1. Pandas Profiling:** Visualizing and understanding the distribution of each variable.

#### **3.5.2. Pairplot:** Seeing correlated features two by two.

#### **3.5.3. Space Study:** Translating a high-dimensional vector into a two dimension space and ploting this to try to see better clusters.

### 3.6. Data Preparation: 

Also called pre processing, consists in "translate" raw data into a language that the model understands. Here I rescaled all features using MinMaxScaler due their non normal distributions and outliers.

### 3.7. Feature Selection: 

Used business knowledge for chose the best features.

### 3.8. Hyperparameter Fine Tunning: 

I tested six K values in three different models using the Silhouette Score as a metric.

### 3.9. Final Model:

Reruned K-Means with 5 clusters ( K ) due the great results.

### 3.10. Cluster Analysis:

Analyzed the performance of the model with Silhouette Plot, Pairplot and UMAP.

### 3.11. Cluster Insights:

Visualized characteristics of each cluster and answered business questions.

## 4.0. Top 3 Data Insights:

- **H1**: Customers with cars below 1 year have more interest in buying vehicle insurance.

**FALSE**. Of the total number of customers interested, the ones with a car younger than 1 year represent only 15.41%.

<img src="img/below_1_year.png" alt="drawing" width="50%"/>

- **H2**: Customers that had their cars damaged have more interest in buying vehicle insurance.

**TRUE**. Almost all customers who are interested in buying vehicle insurance have already had their car damaged.

<img src="img/vehicle_damage.png" alt="drawing" width="50%"/>

- **H3**: Customers with health insurance for more than 100 days have more interest in buying vehicle insurance.

**TRUE**. Of the total number of customers interested, 68,57% have health insurance for more than 100 days.

<img src="img/over_100.png" alt="drawing" width="50%"/>

## 5.0. Machine Learning Models Applied:

- K-Means
- Gaussian Mixture Model ( GMM )
- Hierarchical Clustering

## 6.0. Machine Learning Model Performance:

K-Means with K equal to 5 due the good Silhouette Score.

>>>>>>>> SILHOUETTE PLOT IMAGE <<<<<<<<<<<<

## 7.0. Business Report:

## 8.0. Conclusion:

## 9.0. Next Steps to improve:

- Run the models on embedding space for better score.
- Make a script to rerun the model from time to time and actualize the clusters. Also deploy it on a production environment.
- Predict the revenue of the 'Private' cluster for the next months.

## 10.0. References:

- [Comunidade DS](https://www.comunidadedatascience.com/como-criar-um-programa-de-fidelidade-para-empresa/)
