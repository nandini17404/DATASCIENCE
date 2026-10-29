# Customer Segmentation and Persona Analysis Using Clustering

## 📌 Project Overview

Customer segmentation is a data analysis technique used to group customers based on shared characteristics and purchasing behavior. This project applies unsupervised machine learning techniques to the Mall Customers dataset to identify distinct customer segments based on annual income, spending score, and age.

Using K-Means clustering, hierarchical clustering, and exploratory data analysis, the project identifies customer groups and develops customer personas to support targeted marketing strategies.

## 🎯 Project Objectives

- Analyze customer demographics and spending behavior.
- Identify meaningful customer segments using clustering algorithms.
- Determine suitable cluster counts using the Elbow Method and WCSS.
- Explore customer patterns through 2D and 3D visualizations.
- Develop customer personas based on cluster characteristics.
- Derive insights to support targeted marketing and customer engagement.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy
- **Machine Learning:** Scikit-learn
- **Data Visualization:** Matplotlib, Seaborn, Plotly
- **Techniques:** K-Means Clustering, Hierarchical Clustering, Exploratory Data Analysis (EDA), Feature Scaling, Customer Persona Development

## 📂 Dataset

The project uses the **Mall Customers dataset**, which contains customer information such as:

- Customer ID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

These attributes help explore customer demographics, income levels, and spending behavior.

## ⚙️ Project Workflow

### 1. Data Exploration and Preprocessing

- Examined dataset structure and statistical summaries.
- Explored distributions of age, annual income, and spending scores.
- Visualized relationships between customer attributes.
- Removed `CustomerID` before clustering.
- Applied `StandardScaler` to scale the selected features.

### 2. Exploratory Data Analysis (EDA)

- Used histograms to study feature distributions.
- Created pair plots to examine relationships between variables.
- Generated 2D and 3D visualizations to explore customer behavior patterns.
- Used Plotly for interactive 3D visualization.

### 3. K-Means Clustering

Developed two customer segmentation models:

- **Income and Spending Score:** Applied K-Means clustering with \(k = 5\) to identify customer groups based on annual income and spending behavior.
- **Age and Spending Score:** Applied a separate K-Means model with \(k = 4\) to examine how age relates to spending behavior.

Used the Elbow Method and Within-Cluster Sum of Squares (WCSS) to evaluate the appropriate number of clusters.

### 4. Hierarchical Clustering

- Applied hierarchical clustering using Ward linkage.
- Generated a dendrogram to examine the hierarchical relationships between customers.
- Used a horizontal cutoff at a distance of 6 to explore a five-cluster solution.

### 5. Customer Persona Development

Analyzed cluster characteristics to interpret customer groups and develop customer personas.

The segmentation can help distinguish groups such as:

- **High-Income, High-Spending Customers:** Potential targets for premium offers and loyalty rewards.
- **High-Income, Low-Spending Customers:** Potential opportunities for personalized recommendations and engagement.
- **Low-Income, High-Spending Customers:** Customers who may respond to value-oriented promotions.
- **Low-Income, Low-Spending Customers:** Potential targets for affordable offers and introductory campaigns.
- **Average-Income Customers:** A group that can be further analyzed based on spending behavior.

*Note: These are illustrative persona interpretations. Actual persona labels and characteristics should be aligned with the cluster profiles observed in the analysis.*

## 📊 Key Insights

The project explores how customers differ according to annual income, spending score, and age. Clustering helps reveal groups with similar characteristics, while persona analysis translates these patterns into practical marketing ideas.

The analysis also compares different feature combinations to examine how customer segments change when age is considered alongside spending behavior.

## 💡 Business Applications

- Targeted marketing campaigns
- Personalized product recommendations
- Customer engagement and loyalty programs
- Identification of high-value customer segments
- Customer-focused promotional strategies
- Data-driven marketing decisions

## 🚀 Future Improvements

- Evaluate clustering quality using silhouette scores.
- Compare additional clustering algorithms.
- Develop a customer segmentation dashboard using Power BI.
- Validate customer personas using additional behavioral data.
- Design and evaluate targeted marketing strategies for each segment.

## 👩‍💻 Author

**Nandini Gupta**

- GitHub: [nandini17404](https://github.com/nandini17404)
- LinkedIn: [Nandini Gupta](https://www.linkedin.com/in/nandini-gupta-976aab275/)

---

⭐ If you find this project useful, consider giving the repository a star.
