Mall Customer Clustering Analysis

📌 Project Overview

Customer segmentation is a powerful method for understanding shopping behavior and designing effective marketing strategies.
In this project, mall customers are segmented using demographic, financial, and behavioral attributes.
By applying K-Means and Gaussian Mixture Model (GMM) clustering, the project identifies meaningful customer groups to support targeted marketing and engagement planning.

🎯 Objectives

Group mall customers based on demographic and spending patterns

Analyze behavior using age, income, spending score, and visit-related metrics

Apply K-Means clustering to discover natural customer segments

Use Elbow Method, KneeLocator & Silhouette Score for optimal cluster selection

Support data-driven decisions for marketing, sales, and customer retention

📊 Key Metrics Used

Demographic Metrics
Age
Gender
Age Group
Financial Metrics
Annual_Income_k$
Total_Amount_Spent
Behavioral Metrics
Spending_Score
Visit_Frequency
Avg_Time_Spent_Min
Preferred_Day
Num_Returns
Last_Visit_Days_Ago
Loyalty & Marketing Metrics
Loyalty_Member
Marketing_Opt_In
Payment_Method
These metrics support clustering, RFM analysis, churn prediction, and targeted marketing.

📁 Dataset Overview
Rows: ~5,000 customers
Columns: Demographic, financial, and behavioral attributes
Dataset appears synthetic but realistic and suitable for clustering

Sample Columns
Column	             Description
CustomerID	         Unique identifier
Age, Gender	         Demographic details
Annual_Income_k$	   Yearly income in USD ‘000
Spending_Score	     Normalized spending behavior
Visit_Frequency	     Engagement score
Avg_Time_Spent_Min	 Time spent per visit
Payment_Method	     UPI, Card, Wallet
Loyalty_Member	     Yes/No

🧹 Data Preprocessing
 Missing values checked (none detected)
 Type validation & conversion
 Label Encoding for binary columns
 One-Hot Encoding for categorical features
 Outlier handling with IQR
 Feature scaling (StandardScaler / MinMaxScaler)
 Feature engineering (Income-to-Spend ratio, Engagement score, etc.)

 🔎 Exploratory Data Analysis (EDA)
1️⃣ Gender Distribution – Treemap & Donut Chart
Balanced dataset (Male: 2504, Female: 2496)
Gender-neutral marketing is effective
2️⃣ Age Group Distribution
Seniors form the largest group
Young Adults form the smallest
Useful for age-based personalization
3️⃣ Annual Income Distribution
Even distribution from 20k–150k
Suitable for multi-tiered product segmentation
4️⃣ Spending Score Distribution
Uniform distribution, ideal for clustering
High, medium, and low spenders well represented

🧠 Clustering Approach
1️⃣ Elbow Method (WCSS)
Tested k = 2 to 10
Sharp drop in WCSS followed by flattening
KneeLocator identifies k = 4 as optimal
2️⃣ Silhouette Score
Measures cluster separation quality
Highest silhouette at k = 2
Indicates strong separation at broad group levels
3️⃣ Final Decision
Practical clustering solution used k = 4, supported by Elbow Method and PCA visualization.

📌 K-Means vs GMM
K-Means
Fast, simple, distance-based
Good for spherical clusters
Hard clustering (each point → one cluster)
GMM
Probabilistic soft clustering
Handles overlapping and irregular shapes
More flexible and accurate

🎨 Cluster Visualization
3D PCA Visualization (K-Means)
PCA reduced features to 3 components
Clusters visible with partial overlaps
Cluster counts balanced:
Cluster 1: 1297
Cluster 2: 1232
Cluster 3: 1279
Cluster 4: 1192
GMM Clusters in PCA Space
Captures non-spherical, elliptical cluster shapes that appear in real customer data.
Uses covariance information, so it understands feature relationships better.

💡 Insights & Findings
High spenders are mostly younger, regardless of income
Middle-aged customers show average or low spending
Gender doesn’t strongly influence earning or spending
Income + spending score together form clear natural segments

🖼️ Supporting Visuals
Gender Treemap & Donut Chart
Age Distribution Bar Chart
Income & Spending Histograms
Income vs Spending Score Scatter Plot
Boxplots for outliers
Elbow Curve
Silhouette Score Plot
3D PCA Cluster Visualizations
K-Means vs GMM comparison chart

🚀 How to Use
Steps to run the Mall Customer Clustering Analysis:
1. Clone the Repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
2. Install Dependencies
Make sure you have Python 3.8+ installed, then run:
pip install -r requirements.txt
3. Open the Jupyter Notebook
jupyter notebook Mall.ipynb
4. Load the Dataset
Ensure your dataset (Mall_Customers.xlsx) is in the project folder.
The notebook will load it automatically or use:
df = pd.read_excel("Mall_Customers.xlsx")
5. Run the Notebook Step-by-Step
The notebook performs:
Data Preprocessing
Exploratory Data Analysis (EDA)
Outlier Detection
K-Means Clustering
GMM Clustering
PCA Visualizations
Insights & Findings
6. Export the Final Clustered Data
df.to_excel("clustered_customers.xlsx", index=False)

🛠️ Tools Used
Python 3
Jupyter Notebook
Pandas & NumPy – data processing
Matplotlib & Seaborn – visualizations
Scikit-Learn – K-Means, GMM, PCA, scaling
KneeLocator – elbow point detection
Excel file (.xlsx) for dataset input

📅 Project Duration
November 2025-Decdember 2025.

👩‍💻 Team
Name:Soumya R, Kaushik S, Kaviya R. Project:Mall Customer Clustering Analysis.

📬 Contact
📧 (mailto:soumyarajula280@gmail.com, Kaushiksvh@gmail.com, kaviyaravikumar7@gmail.com)

