# RetailCart ML Engine

*Unsupervised Customer Segmentation & Behavioural Intelligence Platform*


## Executive Summary
**RetailCart ML Engine** is an end-to-end Machine Learning and Customer Analytics designed for e-commerce platforms to transition from generic, "one-size-fits-all" marketing to highly targeted, persona-driven retention strategies. 

By applying **unsupervised clustering algorithms** and **dimensionality reduction (PCA)** on multi-dimensional transactional and demographic data, RetailCart ML Engine automatically partitions customers into distinct behavioral segments, identifies churn risks, and flags high-value VIP shoppers.

---

## The Problem Statement
Modern e-commerce platforms handle thousands of active customer profiles across multiple regions. Operating with blanket marketing strategies leads to critical business bottlenecks:

1. **Capital Inefficiency:** High marketing spend wasted on low-converting audiences.
2. **Revenue Leakage:** Inability to proactively identify, engage, and retain high-value VIP buyers.
3. **Customer Churn:** Delayed detection of disengaged or churn-prone shoppers before they drop off completely.

---

## 🎯 Project Objectives & Aim
* **Data Processing & Feature Engineering:** Transform 22 raw attributes (demographics, purchase history, web activity, campaign response) into high-signal metrics (e.g., Total Spend, Tenure, Household Dynamics).
* **Dimensionality Reduction:** Utilize Principal Component Analysis (PCA) to overcome multicollinearity and compress high-dimensional feature space while retaining maximum variance.
* **Intelligent Clustering:** Benchmark **K-Means**, **Agglomerative Hierarchical Clustering**, and **DBSCAN** to determine optimal mathematical user clusters.
* **Business Personas & Strategy:** Translate raw cluster outputs into actionable customer personas (*Champions*, *Budget Shoppers*, *At-Risk / Churn-Prone*, *Promotional Responders*) with specific marketing workflows.
* **Interactive Dashboard:** Deploy a Streamlit web application enabling real-time segment inspection, scenario filtering, and exportable customer lists.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3.10+
* **Data Processing & Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (StandardScaler, PCA, KMeans, AgglomerativeClustering, DBSCAN)
* **Evaluation Metrics:** Silhouette Score, Davies-Bouldin Index, Inertia (Elbow Method)
* **Visualization:** Matplotlib, Seaborn, Plotly
* **Deployment & UI:** Streamlit / Hugging Face Spaces

---

## Key Features & Engineered Attributes

| Attribute Category | Raw Features | Engineered Features |
| :--- | :--- | :--- |
| **Demographics** | `Year_Birth`, `Education`, `Marital_Status`, `Income` | `Age`, `Living_Status` |
| **Household** | `Kidhome`, `Teenhome` | `Total_Children`, `Has_Children` |
| **Monetary / Spend** | `MntWines`, `MntFruits`, `MntMeat`, `MntFish`, `MntSweets`, `MntGoldProds` | `Total_Spend` |
| **Engagement** | `NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases` | `Total_Purchases` |
| **Campaign Response** | `AcceptedCmp1` through `AcceptedCmp5`, `Response` | `Total_Accepted_Cmps` |
| **Tenure** | `Dt_Customer` | `Tenure_Days` |

---

## 💡 Business Impact & Key Gains
* **Enhanced Retention Rate:** Proactively target high-churn clusters with automated retention offers.
* **Maximized ROI on Marketing:** Eliminate blanket spending by routing campaign budgets exclusively to responsive customer segments.
* **Personalized User Journey:** Tailor product recommendations according to spend behavior and channel preference.

---
