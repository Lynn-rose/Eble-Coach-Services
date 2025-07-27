# 🧠 Customer Segmentation Model – Eble Coach Services

This repository contains a customer segmentation project developed for **Eble Coach Services**, a premium intercity transport provider. The goal of this model is to better understand customer behaviors and value by grouping them into distinct, data-driven segments. These insights are used to drive targeted marketing campaigns, optimize offers, and improve overall customer experience.

---

## 📊 Objective

To replace manual and rule-based customer categorization with a **data-driven segmentation model** using behavioral and transactional data, enabling more effective and scalable customer engagement strategies.

---

## 💡 Approach

We use the **LRFM model** (Length, Recency, Frequency, and Monetary) to define customer value and behavior:

- **Length**: Duration of engagement with Eble Coach Services.
- **Recency**: Days since the last ticket purchase.
- **Frequency**: Number of trips taken.
- **Monetary**: Total amount spent on trips.

---

## ⚙️ Methodology

1. **Data Cleaning**: Standardizing names, emails, dates, and removing invalid records.
2. **Feature Engineering**: Calculating LRFM values from transactional data.
3. **Normalization**: Scaling features appropriately.
4. **AHP Weighting**: Assigning weights to LRFM based on stakeholder input using the Analytic Hierarchy Process.
5. **Clustering**: Segmenting customers using KMeans clustering.
6. **Labeling & Interpretation**: Identifying segment behavior and curating relevant business actions.

---

## 🔍 Segments Identified

- **Premium Customers**
- **High-Value Frequent Flyers**
- **Potential Loyal Customers**
- **At Risk Explorers**

---

## 📁 File Structure
customer-segmentation/
│
├── data/
│ ├── segmentation.csv
│ ├── consent.csv
│ └── matched_customers.csv
│
├── notebooks/
│ ├── customer segmentation.ipynb
│ 
│
├── output/
│ ├── cluster_summary.csv
│ ├── ab_test_groups/
│ ├── premium_treatment.csv
│ ├── premium_control.csv
│ ├── atrisk_treatment.csv
│ └── atrisk_control.csv
│
├── utils/
│ └── ahp_weighting.py
│
├── README.md
└── requirements.txt


---

## 📈 A/B Test Ready

The output of the segmentation is used to:
- Split consented customers into **treatment** and **control** groups.
- Power targeted campaigns for **upsell**, **loyalty**, and **reactivation** strategies.

---

---

## 📊 Dashboard Overview
The results of the customer segmentation were presented in a Power BI dashboard, enabling intuitive exploration of segments, metrics, and customer insights.

1. Customer Segmentation Dashboard

This dashboard provides an overview of customer clusters based on Recency, Frequency, and Monetary values, along with detailed CLV scores.
![Your Image Description](images/image_name.png)


2. Monthly Segment Trend

Tracks how customer segment distributions change over time for better engagement strategy planning.
![Your Image Description](images/image_name.png)


3. Semantics and Segment Definitions

Definitions of key RFM metrics and the behavioral traits used to define each segment.
![Your Image Description](images/image_name.png)


---

## 🛠 Technologies Used

- Python (Pandas, Scikit-learn, NumPy)
- Excel + AHP for Weighting
- Google Tag Manager (for campaign tracking)
- Matplotlib / Seaborn for Visualization

---

## 📝 How to Run

# Install required packages
pip install -r requirements.txt

# Run segmentation notebook
jupyter notebook notebooks/customer segmentation.ipynb

# For more information

Please review my full analysis in my Jupyter Notebook or Eble Coach Services Customer Segmentation Documentation.docs

For any additional questions, please contact Lynn Rose Achieng, lynn90952@gmail.com


