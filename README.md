# ML-Classification  
📅 **Date:** April 02, 2024  
🔍 **Domain:** Banking  
📊 **Topic:** Predictive Modeling for Telemarketing Campaigns

---

## 🔗 [View Full Project Files](https://github.com/Clemobrain/Clem_Portfolio/blob/main/Big%20Data%20And%20Machine%20learning%20Project)

---

## 🧠 Abstract

This project leverages **supervised machine learning classification techniques** to predict whether a customer will subscribe to a term deposit during a Portuguese bank's telemarketing campaign. Using publicly available data from the UCI Machine Learning Repository, the aim is to explore how decision-making can be optimized using AI models like **Random Forest**, **Decision Trees**, and **Boosted Models**.

Key benefits for the bank include:  
- Enhanced targeting of high-potential clients  
- Improved marketing efficiency and ROI  
- Actionable insights on customer behavior  

---

## 📂 Dataset Overview

- **Source:** [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)  
- **Features:** 17 (Categorical & Numerical)  
- **Target:** Binary (`yes` or `no`) — whether a customer subscribed

---

![Azure Dataset Upload](/Photo/subscription.png)
Figure 1: Showing the values for No and Yes class on (subscription) target variable.

---

### 🔑 Variables
- **Demographics:** `age`, `job`, `education`, `marital status`  
- **Campaign Details:** `call duration`, `contact month`, `number of contacts`  
- **Socio-Economic Indicators:** `consumer confidence index`, `employment rate`, `interest rate`

---

## 🧹 Data Preprocessing

- Categorical Encoding with **One-Hot Encoding**
- Standardization with **StandardScaler**
- Feature selection via **RFECV**
- Class imbalance handled using **Random UnderSampling** and **SMOTE**

---


![Azure Dataset Upload](/Photo/Azuredatasetupload.png)


![Convert to Indicator Values - Step 1](/Photo/convert1.png)  

![Convert to Indicator Values - Step 2](/Photo/convert2.png)  

![Correlation Heatmap](/Photo/correlation%20heat%20map.png)  

![Decision Tree Classification Result](/Photo/Decision%20tree%20class.png)  

![Decision Tree Tuning Output](/Photo/decission%20tree%20tune.png)  

![ROC Curve](/Photo/92cb52c8-ddb2-48e2-b043-d286353cf35d.png)  




---

## 📈 Exploratory Data Analysis

The following visuals were generated:

- **Subscription Distribution**
- **Age vs. Subscription**
- **Contact Month vs. Success Rate**
- **Loan Status vs. Subscription**
- **Correlation Heatmap**
- **KDE and Histograms for Continuous Features**

---

## 🤖 Models Implemented

### 1️⃣ Decision Tree Classifier
- **Accuracy:** 80.3%  
- **Issues:** Poor recall on the minority class  
- **Tuned Accuracy:** 82.3%

### 2️⃣ Random Forest Classifier
- **Accuracy:** 83.0%  
- **Tuned Accuracy:** 86.1%  
- **Strengths:** Strong performance on minority class, better generalization

### 3️⃣ Azure ML Boosted Decision Tree
- **AUC:** 0.94  
- **Accuracy:** 90.8%

### 4️⃣ Azure ML Neural Network
- **AUC:** 0.906  
- **Accuracy:** 89.7%

---

## 📊 ROC Curve Visual

```md
![ROC Curve](/Images/roc_classification.png)  
*Figure 1: Comparison of model discrimination power.*
