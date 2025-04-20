# Big-Data-Python-Churn-Project 📉🔍
Customer churn prediction project using Python, Machine Learning (KNN, Decision Trees, Random Forest), and MongoDB integration.

---

## 👥 Team Members:
- **Noa Schneider** 
- **Jenni Shechovitzky** 
- **Emil Raskin** 
---

## 📁 Project Structure:

### 🚩 [Part A: Machine Learning with Python](Part_A_ML_Python/)
Predict customer churn using ML algorithms (KNN, Decision Tree, Random Forest).

**Files included:**
- [**Notebook**: `Churn_KNN_RF_DT.ipynb`](Part_A_ML_Python/Churn_KNN_RF_DT.ipynb)
- [**Presentation**: `python_project_presentation_final.pptx`](Part_A_ML_Python/python_project_presentation_final.pptx)

**Highlights of Part A:**
- Exploratory Data Analysis (EDA)
- Data Cleaning and Preprocessing
- Feature Selection (Correlation threshold: 0.05)
- Model Evaluation:
  - **Best Model:** Random Forest (`n_estimators=151, max_depth=7`)
  - **Accuracy:** Train = **81.72%**, Test = **81.33%**
- Model Interpretation (Feature Importance)

---

### 📌 [Part B: MongoDB Integration](Part_B_MongoDB/)
Integration of MongoDB for data storage and querying with Python.

**MongoDB Setup:**
- Created MongoDB database called `BDA`.
- Created `Customers` collection from provided `churn.json`.

**Notebook:**  
[`Mongo_PartB.ipynb`](Part_B_MongoDB/Mongo_PartB.ipynb)

**Screenshots (MongoDB Compass):**
- Schema Analysis and Cleaning (`6.1.PNG`, `6.2.PNG`)

**Workflow:**
1. Imported data into MongoDB using Compass.
2. Connected to MongoDB via PyMongo.
3. Executed MQL queries to filter complete documents.
4. Imported collection into a Pandas DataFrame.
5. Cleaned data (handled non-scalar fields identified via Compass).
6. Prepared DataFrame for ML.
7. Predicted churn using the best ML model from Part A.
8. Exported results to CSV (`churn_with_predictions.csv`) from notebook.

---

## 🛠️ Technologies & Tools Used:

- Python: Pandas, NumPy, Matplotlib, Scikit-learn, PyMongo
- MongoDB Compass, PyMongo
- Machine Learning: KNN, Decision Tree, Random Forest
- JupyterLab
- PowerPoint for presentation

---

## 🎯 Project Motivation & Goals:
- **Reduce Customer Churn**: Predict customers who may leave.
- **Business Impact**: Lower customer acquisition costs by increasing retention.
- **Insights & Recommendations**: Provide actionable data-driven insights to optimize customer retention strategies.

---

## 📊 Key Findings & Insights:
- **Critical Churn Period**: First 6 months are crucial (churn rate = 52.9%).
- **Contract Impact**: Month-to-month contracts have highest churn (42.7%).
- **High-risk Customers**: Fiber optic users and electronic-check payers.

---

## 🚀 Conclusion & Model Choice:
- **Best Performing Model**: **Random Forest**
  - **Test Accuracy**: 81.33%
  - **Robustness & Interpretability**: Superior handling of complex data patterns and providing insightful feature importance.

---

## 📞 Contact Information:
**Emil Raskin**  
https://www.linkedin.com/in/raskinemil/
