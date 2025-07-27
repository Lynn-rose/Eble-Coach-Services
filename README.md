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
│ ├── segmentation_model.ipynb
│ └── exploratory_analysis.ipynb
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
jupyter notebook notebooks/segmentation_model.ipynb

# For more information

Please review my full analysis in my Jupyter Notebook or my Presentation

For any additional questions, please contact Lynn Rose Achieng, lynn90952@gmail.com


