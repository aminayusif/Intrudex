# Intrudex
📋 Overview
This project performs an end-to-end machine learning analysis to detect cybersecurity intrusions using both supervised and unsupervised learning techniques. It includes:

🧹 Data preprocessing & feature engineering

⚖️ Handling class imbalance

🧠 Training and evaluating classification models

🚨 Detecting anomalies using clustering and isolation-based methods

🔍 Interpreting model predictions using SHAP

The goal is to identify patterns linked to malicious behavior and build models that can effectively flag potential intrusions.

1️⃣ Data Loading & Initial Exploration
🔍 In this step:

Load the dataset

Inspect data types and missing values

Explore initial trends and distributions

2️⃣ Data Preprocessing & Feature Engineering
🛠️ Key tasks:

Drop irrelevant columns (e.g., session_id)

Handle missing values (encryption_used)

Create derived features like failed_login_ratio

Add polynomial features to capture nonlinear behavior

3️⃣ Handling Class Imbalance
⚖️ The dataset shows imbalance in the target variable (attack_detected):

SMOTE is used to oversample the minority class

Visualizations show class distribution before and after balancing

4️⃣ Supervised Learning (Model Training & Evaluation)
🧠 Algorithms Used:

Logistic Regression

Random Forest

Decision Tree

XGBoost

🔧 Key processes:

Train/Test split & hyperparameter tuning (GridSearchCV)

Evaluation using accuracy, precision, recall, F1-score, and ROC AUC

ROC curves plotted for all models

5️⃣ Unsupervised Learning (K-Means & Isolation Forest)
🚫 This section focuses on anomaly detection techniques:

🌀 K-Means Clustering
Group data into clusters

Use Elbow method to find optimal k

Visualize using PCA

🌲 Isolation Forest
Detect outliers using tree-based isolation

Visualize normal vs. anomalous traffic

6️⃣ Model Interpretation with SHAP
🔍 SHAP (SHapley Additive exPlanations) explains model predictions:

Summary plot shows feature importance

Force plot highlights how each feature impacts anomaly scores

Adds transparency and trust to the models

7️⃣ Summary & Conclusion
📌 Key Takeaways:

Supervised models were effective in detecting known intrusions

Unsupervised techniques revealed novel or rare threats

SHAP enhanced interpretability of anomaly detection

📈 Next steps may include deep learning, real-time detection, or system deployment

 

📦 Dependencies
Install required packages:

 
pandas, numpy, scikit-learn, xgboost, imbalanced-learn, matplotlib, seaborn, shap

Potential next steps:

Integrate deep learning (e.g., Autoencoders, LSTMs)

Real-time anomaly detection systems

Deploy models for live traffic monitoring

📂 Project Status
✅ Completed core analysis and modeling
🚧 Future work may include deep learning, real-time data pipelines, or integration with SIEM tools.

 
