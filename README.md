# 🍷 Wine Quality Classification Using SVM (RBF Kernel)
Predict wine quality using SVM with RBF kernel. Includes data preprocessing, SMOTE for imbalance handling, hyperparameter tuning, and model evaluation with precision, recall, and F1-score metrics.

---

## 📝 Project Overview
This project predicts wine quality using a **Support Vector Machine (SVM) with RBF kernel**.  
The dataset contains physicochemical tests of wines. The task is simplified into a **binary classification**:

- **Good wine (1):** quality ≥ 6  
- **Bad wine (0):** quality < 6  

We use **SMOTE** to handle class imbalance and **GridSearchCV** for hyperparameter tuning.

---

## 📊 Dataset
- Publicly available dataset: [Wine Quality Dataset](https://raw.githubusercontent.com/Explore-AI/Public-Data/master/Data/classification_sprint/winequality.csv)  
- Features: `fixed acidity`, `volatile acidity`, `citric acid`, `residual sugar`, `chlorides`, `free sulfur dioxide`, `total sulfur dioxide`, `density`, `pH`, `sulphates`, `alcohol`  
- Target: `quality` (converted to binary)

---

## 🛠️ Tools & Libraries
- Python 3, Jupyter Notebook  
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn (SVM, GridSearchCV, Pipeline)  
- imbalanced-learn (SMOTE)  

---

## 🚀 Workflow
1. **Data Loading & Exploration** – Inspect dataset, handle missing values.  
2. **Preprocessing** – Impute missing values, convert target to binary, scale features.  
3. **Train-Test Split** – 80% train, 20% test, stratified by target.  
4. **Modeling** – SVM with RBF kernel using a pipeline (Imputer → SMOTE → Scaler → SVM).  
5. **Hyperparameter Tuning** – GridSearchCV to find optimal `C` and `gamma`.  
6. **Evaluation** – Accuracy, classification report, confusion matrix.

---

## 📈 Results

- **Best Parameters:** `C=1`, `gamma=1`, `kernel='rbf'`  
- **Cross-Validation Accuracy:** 78.47%  
- **Test Accuracy:** 78.46%  

**Classification Report**
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.70      | 0.72   | 0.71     | 477     |
| 1     | 0.84      | 0.82   | 0.83     | 823     |

**Overall Accuracy:** 0.78  
**Total Test Samples:** 1300

---

## 📬 Contact  
Created by FELLAH HANANE

📧 Email: hananefellah35@gmail.com

🌐 GitHub: hananefellah

## 📄 License  
MIT License  
---
