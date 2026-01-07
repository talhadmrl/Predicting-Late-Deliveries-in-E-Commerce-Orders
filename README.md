Youtube link: https://www.youtube.com/watch?v=VlyZWg6KT6o

#  Predicting Late Deliveries in E-Commerce Orders

##  Project Overview  
This project aims to build a **machine learning classification model** to predict whether an e-commerce order will be **delivered on time or late**.  
Using real-world Brazilian e-commerce data, the model identifies potential delivery delays based on customer, product, payment, and logistical information.  

Predicting late deliveries can help online retailers **improve logistics, manage customer expectations, and optimize delivery performance**.

---

##  Dataset Description  
**Dataset:** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)  
This dataset contains real order data from the Olist platform — one of Brazil’s largest marketplaces.  
It includes detailed information about orders, products, payments, sellers, and customer locations.

**Main CSV files used:**
- `olist_orders_dataset.csv`  
- `olist_order_items_dataset.csv`  
- `olist_customers_dataset.csv`  
- `olist_order_reviews_dataset.csv`  

These files are merged to create a unified dataset.  
A target variable named **`delivered_late`** is generated to represent whether each order was delivered late (`1`) or on time (`0`).

---

##  Problem Definition  
The goal is to **classify each order** as either:
- `0` → Delivered on time  
- `1` → Delivered late  

This is a **binary classification problem**, where the model predicts the probability of late delivery based on multiple order-related features.

---

##  Data Preprocessing & Feature Engineering  
Before training models, several data preparation and transformation steps are performed:

1. **Handling missing values** using median or mode  
2. **Removing outliers**, e.g., dropping records with `price > 1500`  
3. **Encoding categorical variables** using One-Hot Encoding  
4. **Addressing class imbalance** (approx. 95%-5% distribution)  
5. **Feature scaling** using `StandardScaler`  
6. **Splitting data** into training (80%) and testing (20%) sets  

---

##  Machine Learning Models  
Multiple classification algorithms are applied and compared to evaluate performance differences:

| Algorithm | Description |
|------------|--------------|
| **Logistic Regression** | Baseline linear classifier for binary problems |
| **Decision Tree Classifier** | Tree-based model that splits features into decision rules |
| **Random Forest Classifier** | Ensemble of multiple trees to reduce overfitting |
| **Support Vector Machine (SVM)** | Finds the optimal hyperplane that separates classes |
| **K-Nearest Neighbors (KNN)** | Instance-based algorithm based on similarity between samples |
| **Naive Bayes Classifier** | Probabilistic model effective for categorical features |

---

##  Evaluation Metrics  
To assess model performance, the following metrics are calculated:

- **Accuracy** — Overall correctness of predictions  
- **Precision** — Proportion of correctly predicted positive cases  
- **Recall (Sensitivity)** — Ability to detect all positive cases  
- **F1 Score** — Harmonic mean of precision and recall  
- **Confusion Matrix** — Visual representation of true vs predicted labels  

---

##  Project Pipeline  

1. **Data Loading & Integration**  
2. **Exploratory Data Analysis (EDA)**  
3. **Feature Engineering & Preprocessing**  
4. **Model Training & Tuning**  
5. **Model Comparison & Evaluation**  
6. **Conclusion & Insights**

---

##  Technologies Used  
- **Python 3.10+**  
- **Pandas, NumPy, Scikit-learn**  
- **Matplotlib, Seaborn** (for visualization)  
- **Jupyter Notebook / Google Colab**

---


