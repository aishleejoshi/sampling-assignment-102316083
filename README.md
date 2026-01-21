# Sampling Assignment – Machine Learning

This project analyzes the impact of different sampling techniques on the
performance of multiple machine learning models using an imbalanced dataset.

---

## 📌 Objective
- Convert an imbalanced dataset into a balanced dataset
- Apply multiple sampling techniques
- Train different machine learning models
- Compare model performance across sampling methods

---

## 📂 Dataset
- Credit Card Transaction Dataset
- Highly imbalanced binary classification problem
- Target variable: `Class`

---

## 🔄 Methodology & Pipeline

### 1️⃣ Data Preprocessing
- Loaded dataset using Pandas
- Checked missing values and data types
- Separated features and target variable

### 2️⃣ Feature Scaling
- Applied **StandardScaler** to normalize feature values

### 3️⃣ Oversampling
- Used **SMOTE (Synthetic Minority Over-sampling Technique)**
- Balanced the dataset by generating synthetic minority samples

### 4️⃣ Sampling Techniques Applied
Five sampling techniques were applied to the balanced dataset:

1. Simple Random Sampling  
2. Systematic Sampling  
3. Stratified Sampling  
4. Cluster Sampling  
5. Bootstrap Sampling  

For each technique, class distribution was analyzed **before and after sampling**.

---

## 🤖 Machine Learning Models Used

Five models from different learning paradigms were selected:

- Logistic Regression  
- Decision Tree Classifier  
- Random Forest Classifier  
- K-Nearest Neighbors (KNN)  
- Support Vector Machine (SVM)  

---

## 📊 Model Evaluation
- 5-fold Cross Validation was used
- Accuracy was chosen as the evaluation metric
- Each model was trained on each sampled dataset

---

## 🏆 Results
- An accuracy comparison table was generated
- The best sampling technique for each model was identified
- Results show that no single sampling technique is optimal for all models

---

## 🧠 Conclusion
The experiment demonstrates that model performance is highly dependent on the
sampling strategy used. Stratified and bootstrap sampling techniques generally
produced better results for most models.

---

## 🛠 Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn
- Google Colab

---

## 📎 Author
Aishlee Joshi
