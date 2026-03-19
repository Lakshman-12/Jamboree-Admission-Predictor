# 🎓 Jamboree Admission Predictor

## 📌 Problem Statement

This project aims to predict the probability of a student getting admission into top universities based on key academic and profile features such as **GRE Score, TOEFL Score, CGPA, SOP, LOR, University Rating, and Research Experience**.

---

## 📊 Dataset Overview

* 📁 Total Records: 500
* 📌 Features:

  * GRE Score
  * TOEFL Score
  * University Rating
  * SOP (Statement of Purpose)
  * LOR (Letter of Recommendation)
  * CGPA
  * Research (0/1)
  * Chance of Admit (Target Variable)

---

## 🔍 Exploratory Data Analysis (EDA)

### Key Insights:

* 📈 **GRE, TOEFL, CGPA** → Strong positive impact on admission chances
* 📊 **SOP, LOR, University Rating** → Moderate influence
* 🔬 **Research Experience** → Improves admission probability
* 📉 Most students have **high academic scores** (strong dataset)

---

## 📈 Data Preprocessing

* Removed unnecessary column: `Serial No.`
* No missing values found ✅
* No duplicate records ✅
* Feature scaling applied using **StandardScaler**

---

## ⚙️ Feature Engineering

* Created:

  * `Overall_Score = GRE + TOEFL`
  * `SOP_LOR_Interaction = SOP × LOR`
* ❌ Removed due to multicollinearity (based on VIF)

---

## 🤖 Model Building

### 1️⃣ Linear Regression

* Trained on 80% data
* Tested on 20% data

### 📊 Performance:

* **R² Score: 0.82**
* Strong prediction capability

---

### 2️⃣ Ridge Regression (Final Model)

* Used to handle multicollinearity
* Applied L2 Regularization

### 📊 Performance:

* **R² Score: ~0.82 (same as Linear)**
* More stable and reliable coefficients ✅

---

## 📉 Model Evaluation

* Predictions closely match actual values
* Residuals are randomly distributed (good fit)
* No major outliers found

---

## 🔑 Key Findings

* 🎯 **CGPA is the most important factor**
* 📊 GRE & TOEFL also strongly influence admission
* 📝 SOP & LOR provide additional support
* 🔬 Research experience increases chances

---

## 🏁 Conclusion

* Academic performance is the **primary factor** for admission
* Ridge Regression is the **best model** due to:

  * Handling multicollinearity
  * Maintaining performance
  * Better coefficient stability

---

## 🛠️ Tech Stack

* Python 🐍
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🚀 How to Run

1. Clone the repository
2. Open the `.ipynb` file in Jupyter/Colab
3. Run all cells

---

## 📌 Future Improvements

* Try advanced models (Random Forest, XGBoost)
* Hyperparameter tuning
* Deploy as a web app (Streamlit)

---

## 👨‍💻 Author

**Lakshman (Lucky)**
B.Tech - AI & Data Science

---
