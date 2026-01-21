# Sampling Assignment – PREDICTIVE ANALYSIS(UCS654)

This project analyzes the impact of different sampling techniques on the
performance of multiple machine learning models using an imbalanced dataset.
---

## 🎯 Objective

The objectives of this assignment are:

- To handle **class imbalance** in a real-world dataset
- To apply **SMOTE oversampling** to balance the dataset
- To generate multiple datasets using **sampling techniques**
- To evaluate **five machine learning models**
- To compare model performance using **accuracy tables**

---

## 📊 Dataset Description

- Dataset: Credit Card Transactions
- Target variable: `Class`
  - `0` → Non-fraudulent transaction
  - `1` → Fraudulent transaction
- Nature of data: Highly imbalanced

### Original Class Distribution
- Majority class: Class 0
- Minority class: Class 1

This imbalance motivates the use of oversampling techniques.

---

## ⚖️ Class Balancing Using SMOTE

SMOTE (Synthetic Minority Oversampling Technique) is applied to the **entire
dataset** to address class imbalance.

### Why SMOTE?
- Prevents model bias toward the majority class
- Generates synthetic minority class samples
- Improves learning for rare class patterns

After applying SMOTE, both classes have equal representation, which forms the
base dataset for further sampling.

---

## 🔁 Sampling Techniques Applied

After balancing, the following sampling techniques are applied:

1. **Simple Random Sampling**
   - Random selection of observations from the dataset

2. **Systematic Sampling**
   - Selection of every k-th data point

3. **Stratified Sampling**
   - Ensures proportional representation of classes

4. **Cluster Sampling**
   - Data divided into clusters, one cluster selected

5. **Bootstrap Sampling**
   - Sampling with replacement from the dataset

For each technique, **before and after class distributions are printed**
to show the effect of sampling.

---

## 🤖 Machine Learning Models Used

Each sampled dataset is evaluated using the following models:

| Model ID | Algorithm |
|--------|----------|
| M1 | Logistic Regression |
| M2 | Decision Tree |
| M3 | Random Forest |
| M4 | K-Nearest Neighbors |
| M5 | Support Vector Machine |

---

## 📈 Model Evaluation Methodology

- Metric used: **Accuracy**
- Evaluation method: **5-fold cross-validation**
- Each model is trained and evaluated on **each sampled dataset**
- Mean accuracy values are computed and stored in a table

---

## 📋 Result Table Explanation

The final output is an **accuracy comparison table**, where:

- **Rows** represent machine learning models
- **Columns** represent sampling techniques
- **Cell values** indicate mean accuracy (%) obtained from cross-validation

### Interpretation:
- Higher accuracy indicates better model performance
- For each model, the sampling technique with the **highest accuracy** is
  considered the best choice

---

## 🏆 Best Sampling Technique per Model

Using the accuracy table, the best sampling technique is identified for
each model by selecting the column with the maximum accuracy value per row.

This allows a clear comparison of how different sampling methods influence
model performance.

---

## ✅ Key Observations

- Class imbalance significantly affects model accuracy
- SMOTE effectively balances the dataset
- Sampling techniques impact models differently
- Ensemble models like Random Forest show consistently strong performance
- No single sampling technique is universally optimal

---

## 🛠 Tools & Libraries Used

- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)

---
---

## 👩‍💻 Author

**Name:** Aishlee Joshi  
**Enrollment / Roll No:** 102316083  
**Course:** PREDICTIVE ANALYSIS   
**Institution:** Thapar Institute of Engineering & Technology  

---


## 📌 Conclusion

This assignment demonstrates the importance of class balancing and sampling
strategies in machine learning. By systematically applying multiple sampling
techniques and models, the study highlights how preprocessing decisions
directly influence predictive performance.

