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

![subscription](/Photo/subscription.png)
Figure 1: Showing the values for No and Yes class on (subscription) target variable.

---

![subscription status](/Photo/subscription%20status.png)
Figure 2: It shows that persons within 30 years subscribe the most.

---

![subscription per month](/Photo/subscription%20per%20month.png)
Figure 3: This code uses a bar chart with stylised formatting to compute and display subscription rates by month. The month of march has highest subscription rates.

---

![frequency of jobs](/Photo/frequency%20of%20jobs.png)
Figure 4:The categorical features analysis shows histograms and KDE plots of the distribution of continuous features.  

---

![correlation heat map](/Photo/correlation%20heat%20map.png)
Figure 5:Calculated numerical features for correlations, visualising and to view them interactively for insights into relationships.

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

![onehotencoding](/Photo/onehotencoding1map.png)

---

![onehotencoding](/Photo/onehotencoding.png)
Figure 6: Firstly I removed the target variable and deleted the dummy class variables I used for visualisation. The dataset categorical variables are fully encoded as one-hot-encoded features and ready for modelling.

---

![spliting](/Photo/split.png)
![spliting](/Photo/split2.png)
Figure 7:  Above I defined my features and target, I then converted my target “y” from (yes to 1 and no to 0) Splitting all feature into ‘X’ and target variable to ‘y’

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
