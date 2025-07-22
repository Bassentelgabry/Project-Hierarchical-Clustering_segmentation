# 🎯 Customer Segmentation using Hierarchical Clustering

This project applies **unsupervised learning** to segment customers based on their purchasing behavior and demographic information. Then, we use a **supervised model** to predict the customer cluster. The dataset comes from a real-life marketing campaign.

---

## 📊 Objective

Segment customers into meaningful groups to:
- Discover high-value segments
- Target low-engagement customers with personalized strategies
- Predict cluster for new users based on key features

---

## 📁 Dataset Overview

**Source:** `marketing_campaign.csv`

**Features used:**
- Income
- Total Spending on products
- Number of Accepted Campaigns
- Total Purchases (Web, Store, Catalog, Deals)
- Kidhome, Teenhome
- Age (calculated from Year_Birth)

---

## 🧠 Methods Used

- 📌 Exploratory Data Analysis (EDA)
  - Heatmap
  - Boxplots
  - Pairplot
- 📌 Feature Engineering
  - Total Spending
  - Total Purchases
  - Total Accepted Campaigns
  - Age group segmentation
- 📌 Scaling
  - RobustScaler (for Income, Spending, Campaigns)
  - StandardScaler (for discrete features)
- 📌 Clustering
  - Hierarchical Clustering (`AgglomerativeClustering`)
  - PCA for visualization
- 📌 Prediction
  - Decision Tree Classifier to predict cluster of new customer

---

## 📌 Cluster Profiles – Marketing Insight by Age Group

### 🎯 Cluster 0: High Income, High Spending — **Premium Customers**
- Marketing Strategy: Loyalty programs, VIP offers, exclusive bundles  
- Common Age Group: **30–50 years**  
- Best Channels: Mobile apps, Email automation

---

### 💤 Cluster 1: Low Income, Low Spending — **Passive or Budget-Constrained**
- Marketing Strategy: Deep discounts, Flash sales, Entry-level products  
- Common Age Group: **20–35 years**  
- Best Channels: Social media ads, SMS campaigns

---

### 💡 Cluster 2: Medium Income, High Spending — **Value Seekers**
- Marketing Strategy: Smart bundles, targeted promotions  
- Common Age Group: **35–55 years**  
- Best Channels: Google Ads, Email marketing

---

### 📉 Cluster 3: High Income, Low Spending — **Untapped Potential**
- Marketing Strategy: Highlight product value, emotional branding  
- Common Age Group: **45+ years**  
- Best Channels: Webinars, social proof, testimonials

---

### 🧩 Cluster 4: Mixed Behavior — **Transitional Segment**
- Marketing Strategy: A/B testing, behavioral analysis  
- Common Age Group: Varied  
- Note: May require further sub-segmentation
  
## 🔮 Predicting New Customers

After clustering, we trained a **Decision Tree Classifier** to predict which cluster a new customer would belong to — based on:

- Income  
- Total Spend  
- Total Accepted Campaigns  
- Total Purchases

✅ A simple input interface is provided for testing.

## 📸 Visualizations

- Dendrogram (Hierarchical Clustering Tree)
- PCA 2D Cluster Map (with new custome
