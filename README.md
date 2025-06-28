# 📊 Bank Marketing – Decision Tree Classifier (Internship Task)

This project fulfills my Data Science internship task at **Prodigy InfoTech**, where I built and evaluated a Decision Tree classifier on the Bank Marketing dataset to predict whether a client will subscribe to a term deposit.

---

## 📁 Dataset Used

- **Source**: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- **Version**: `bank.csv` with **4,521 rows** and **17 columns**
- **Target Variable**: `y` (yes/no – whether the client subscribed)

---

## 🧪 Methodology

1. **Data Preprocessing**
   - Categorical columns label-encoded using `LabelEncoder`
   - Handled class imbalance using `class_weight='balanced'`
   - Train-test split: 80/20, stratified on target variable

2. **Model**
   - `DecisionTreeClassifier` from `sklearn`
   - Max depth: **4** (to improve readability and reduce overfitting)

3. **Evaluation Metrics**
   - Accuracy, precision, recall, F1-score
   - Confusion matrix
   - Feature importance analysis

---

## ✅ Results

| Metric        | Value     |
|---------------|-----------|
| **Accuracy**  | 72.9%     |
| **Recall (yes)** | 0.85  |
| **Precision (yes)** | 0.28 |

📌 The model detects most of the “yes” responses (high recall), but also has many false positives (low precision) due to class imbalance.

---

## 🌳 Key Features

- **Top predictors**: `duration`, `pdays`, `contact`, `month`
- Visualizations include:
  - Class distribution
  - Decision tree (limited to depth 4)
  - Confusion matrix
  - Feature importance bar chart

---

## 💡 How to Run

1. Upload the `bank.zip` file (or `bank-additional.zip` for full dataset)
2. Open and run the notebook in JupyterLab or Colab
3. The notebook will automatically extract, preprocess, train, and visualize

---

## 📌 Internship Info

**Internship Provider**: Prodigy InfoTech  
**Task**: Build and evaluate a classification model using real-world data

---

> ✨ *This project helped me understand how machine learning models work on real, imbalanced datasets and how to evaluate them effectively.*

# PRODIGY_DS_03
