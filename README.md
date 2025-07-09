# Google Data Analytics Capstone Case Study

## Customer Segmentation Analysis using Machine Learning

---

## Introduction

Welcome to my case study for the Google Data Analytics Capstone. This project focuses on leveraging data analysis and machine learning to understand customer behavior and provide actionable insights for business decision-making. My goal is to showcase my skills in defining a business problem, preparing and processing data, performing analysis, and effectively sharing findings, ultimately creating a portfolio-ready case study.

---

## ASK

**Business Task:**  
A retail mall seeks to better understand customer behavior to enable targeted marketing. The goal is to segment customers based on demographic and spending patterns using unsupervised machine learning (K-means clustering).

**Stakeholders:**  
- Mall marketing team  
- Sales and promotions department  
- BI analysts

**Key Questions:**
- Can we segment mall customers based on age, income, and spending?
- What patterns or behaviors define these groups?
- How can these insights guide marketing strategies?

**Audience:**  
The client and internal stakeholders interested in consumer insights. The final presentation includes visualizations, summary findings, and actionable recommendations.

---

## PREPARE

**Dataset:**  
- **File**: `Mall_Customers.csv`  
- **Source**: Public Kaggle dataset

**Features Used:**  
- Age  
- Annual Income (USD)  
- Spending Score (1–100)  
- Gender (exploratory only)

**ROCCC Check:**
- **Reliable**: Consistent and stable data  
- **Original**: Public dataset widely referenced  
- **Comprehensive**: Key attributes present for segmentation  
- **Current**: Suitable for demonstration despite undated records  
- **Cited**: Referred to as `Mall_Customers.csv`

---

## PROCESS

**Tools:**  
- R (tidyverse, ggplot2, cluster, factoextra)

**Cleaning Steps:**
- Loaded and inspected the dataset  
- Verified column names and data types  
- Checked for missing values (none found)  
- Conducted univariate visualizations to confirm readiness for clustering

---

## ANALYZE

**Univariate Analysis:**
- Gender distribution (bar chart, pie chart)
- Age, Income, Spending Score (histograms, boxplots, density curves)

**Clustering Preparation:**
- **Elbow Method**: Suggested k = 5 or 6  
- **Silhouette Score**: Highest at k = 6  
- **Gap Statistic**: Confirmed k = 6

**Clustering (K-means with k=6):**
- PCA used for dimensionality reduction
- Cluster visualization using scatter plots and PCA projections

**Cluster Profiles:**
1. **High Income, Low Spend** – Affluent but frugal  
2. **Moderate Income, High Spend** – Loyal middle-income buyers  
3. **Low Income, Low Spend** – Budget-conscious shoppers  
4. **High Income, High Spend** – VIP/high-value customers  
5. **Young, Low Income, Moderate Spend** – Trend-driven spenders  
6. **Older, Moderate Income, Low Spend** – Less active seniors

---

## SHARE

**Visualizations Used:**
- Gender pie/bar chart
<br> ![image](https://github.com/user-attachments/assets/c8f95ada-85d5-4a8c-a8dd-6115ea1521ba)
![image](https://github.com/user-attachments/assets/da70f810-d9ec-4fa7-b50c-bf6ef01525db)

- Age, income, spending score histograms/boxplots
<br> ![image](https://github.com/user-attachments/assets/c5ae3177-3e93-45e8-96a2-a351467f3eb3)
![image](https://github.com/user-attachments/assets/09f2d059-67e0-4167-81da-35c209fed59c)
<br> ![image](https://github.com/user-attachments/assets/d9c00c3f-fe09-40b5-ae8e-17382a5003fd)
![image](https://github.com/user-attachments/assets/df63e80e-2135-4ed6-8fe7-159bbf5f8b39)
<br> ![image](https://github.com/user-attachments/assets/20cf109f-d047-407f-a67c-e684ba6c1aae)

- Elbow and silhouette plots
<br> ![image](https://github.com/user-attachments/assets/c6bdbabc-84db-454f-a07a-8a28c1d59491)
![image](https://github.com/user-attachments/assets/8b27ff49-2acf-4095-8c77-bec950f929bc)

- PCA-based 2D cluster visualizations
<br> ![image](https://github.com/user-attachments/assets/182c6697-31da-4efc-b492-e949ef4a674e)

- Income vs. Spending Score, Age vs. Spending Score scatter plots
<br> ![image](https://github.com/user-attachments/assets/17bf3976-3c80-47ed-86b1-371e6731c9da)
![image](https://github.com/user-attachments/assets/6c5fd6bd-f36e-434a-b989-acea8582ba12)

**Key Findings:**
- Cluster 4 (high-high) is the highest value group  
- Cluster 3 (low-low) represents the budget-conscious  
- Younger customers tend to spend more despite lower incomes  
- Gender was not a major driver of behavior differences

---

## ACT

**Top Insights:**
- K-means clustering revealed 6 distinct segments  
- Cluster 4 should be prioritized for premium campaigns  
- Cluster 1 (affluent but frugal) offers upselling potential  
- Cluster 5 (young, trend-driven) can be engaged with affordable, stylish offers  
- Marketing strategies can remain gender-neutral

**Further Recommendations:**
- Perform Customer Lifetime Value analysis  
- Run market basket analysis per cluster  
- Build churn prediction models  
- Test campaign impact per cluster  
- Incorporate time-series spending trends  
- Overlay geographic data if available

---

## 📁 Project Info

**Tools:** R, tidyverse, ggplot2, cluster, factoextra  
**Skills Demonstrated:** Data cleaning, clustering, PCA, EDA, visualization  
**Status:** Capstone project for the Google Data Analytics Certificate

---

## Conclusion

This project successfully implemented K-means clustering to segment mall customers based on their age, income, and spending behavior. By combining exploratory data analysis, clustering validation techniques, and advanced visualizations, it revealed actionable customer segments useful for business decision-making. The six identified clusters provide valuable insights for targeted marketing. This type of segmentation forms the basis for customer profiling, campaign personalization, and data-driven marketing strategies. The application of clustering and PCA in this context illustrates the power of unsupervised learning in real-world business analytics.
