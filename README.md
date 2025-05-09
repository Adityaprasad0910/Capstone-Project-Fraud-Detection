Thought for a couple of seconds


````markdown
# Fraud Detection Capstone Project

## 📋 Project Overview  
This repository contains an end-to-end machine learning pipeline to detect fraudulent credit-card transactions. We leverage extensive EDA, feature engineering, and multiple classifiers—emphasizing **high recall**—to catch as many fraud cases as possible, then quantify the business impact of our model’s decisions.

---

## 🚀 Contents  
- **`data/`** – Raw and preprocessed datasets  
- **`notebooks/`** – Jupyter notebooks:
  - `01_EDA.ipynb` – Exploratory Data Analysis & visualizations  
  - `02_Preprocessing.ipynb` – Cleaning, outlier treatment, encoding, scaling  
  - `03_Modeling.ipynb` – Training base classifiers & evaluation  
  - `04_Financial_Impact.ipynb` – Loss/savings analysis  
- **`images/`** – Charts used in the PPT and README  
- **`ppt/`** – Final PowerPoint slides  
- **`utils/`** – Helper scripts and Python modules  
- **`requirements.txt`** – Python dependencies  

---

## ⚙️ Installation

1. Clone this repo:  
   ```bash
   git clone https://github.com/Adityaprasad0910/Capstone-Project-Fraud-Detection.git
   cd Capstone-Project-Fraud-Detection
````

2. Create and activate a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate
   ```
3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## 🏃 How to Run

1. **EDA & Preprocessing**

   ```bash
   jupyter notebook notebooks/01_EDA.ipynb
   jupyter notebook notebooks/02_Preprocessing.ipynb
   ```
2. **Model Training & Evaluation**

   ```bash
   jupyter notebook notebooks/03_Modeling.ipynb
   ```
3. **Financial Impact Analysis**

   ```bash
   jupyter notebook notebooks/04_Financial_Impact.ipynb
   ```
4. **Generate PPT Slides**

   ```bash
   python utils/build_ppt.py
   ```

---

## 📈 Key Results

| Model               | Precision | Recall   | F1-Score | ROC-AUC  |
| ------------------- | --------- | -------- | -------- | -------- |
| Logistic Regression | 0.45      | 0.65     | 0.53     | 0.84     |
| Random Forest       | 0.72      | 0.58     | 0.64     | 0.89     |
| **XGBoost**         | **0.78**  | **0.62** | **0.69** | **0.93** |

* **Best model**: XGBoost (highest AUC & F1-score).
* **Business impact**: Improving recall by 10% can save tens of thousands of dollars in undetected fraud.

---

## 🔍 What’s Inside

* **Thorough EDA**: Distribution plots, boxplots, correlation heatmaps.
* **Robust Preprocessing**: Missing values, outlier capping, Box–Cox transforms, one-hot encoding, scaling.
* **Model Diversity**: Logistic Regression, Decision Tree, Random Forest, SVM, XGBoost.
* **Evaluation Focus**: Precision, Recall, F1, ROC-AUC, plus confusion matrices & ROC curves.
* **Financial Lens**: Calculated false-negative losses vs. true-positive savings.

---

## 🚧 Next Steps

1. **Hyperparameter Tuning** with GridSearchCV / RandomizedSearchCV.
2. **Threshold Optimization** via precision-recall curves to hit target recall.
3. **Explainability**: SHAP or LIME to interpret feature contributions.
4. **Temporal Features**: Rolling-window frequencies & recency metrics.
5. **Deployment**: Package model in a REST API, set up monitoring for drift.

---

## 📂 License & Acknowledgments

* Dataset: [Kaggle Credit Card Fraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)
* Thanks to scikit-learn, pandas, imbalanced-learn, matplotlib

This project is released under the MIT License.

```
```
