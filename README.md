# Maincrafts AI/ML Task 4 – Classification Models

## 📌 Project Overview

This project is part of the **Maincrafts Technology Artificial Intelligence & Machine Learning Internship – Task 4**.

The objective is to build and evaluate binary classification models using the **Breast Cancer Dataset** and compare their performance using multiple evaluation metrics.

## 🎯 Objectives

* Build a binary classification system.
* Implement Logistic Regression.
* Handle class imbalance using `class_weight="balanced"`.
* Implement a Decision Tree classifier.
* Generate a confusion matrix.
* Calculate Accuracy, Precision, Recall and F1-score.
* Plot ROC curves and calculate AUC.
* Compare the performance of different classification models.
* Select the most suitable model based on the evaluation results.

## 📊 Dataset

The project uses the **Breast Cancer Wisconsin Diagnostic Dataset** available through `scikit-learn`.

The dataset contains:

* **569 samples**
* **30 numerical features**
* **2 target classes**

  * `0` – Malignant
  * `1` – Benign

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

## 🤖 Machine Learning Models

### 1. Logistic Regression

Used as the baseline classification model.

### 2. Balanced Logistic Regression

A second Logistic Regression model was trained using:

```python
class_weight="balanced"
```

This helps reduce the effect of class imbalance.

### 3. Decision Tree

A Decision Tree classifier was trained and compared with the Logistic Regression models.

## ⚙️ Methodology

```text
Load Dataset
     ↓
Data Preparation
     ↓
Train/Test Split (80/20)
     ↓
Feature Scaling
     ↓
Logistic Regression
     ↓
Confusion Matrix & Classification Report
     ↓
ROC Curve & AUC
     ↓
Handle Class Imbalance
     ↓
Decision Tree
     ↓
Model Comparison
     ↓
Final Model Selection
```

## 📈 Evaluation Metrics

The models were evaluated using:

| Metric    | Purpose                                              |
| --------- | ---------------------------------------------------- |
| Accuracy  | Measures overall correctness                         |
| Precision | Measures correctness of positive predictions         |
| Recall    | Measures how many actual positive cases are detected |
| F1-Score  | Balance between precision and recall                 |
| ROC-AUC   | Measures classification discrimination ability       |

For medical classification, **Recall** is particularly important because false-negative predictions can be critical.

## 📊 Model Performance

| Model                        |   Accuracy | Precision |     Recall |   F1-Score |        AUC |
| ---------------------------- | ---------: | --------: | ---------: | ---------: | ---------: |
| Logistic Regression          | **98.25%** |    98.61% | **98.61%** | **98.61%** | **0.9954** |
| Balanced Logistic Regression |     95.61% |    98.55% |     94.44% |     96.45% |     0.9954 |
| Decision Tree                |     91.23% |    95.59% |     90.28% |     92.86% |     0.9157 |

## 🏆 Final Model

Based on the experimental results, **Logistic Regression** achieved the best overall performance.

It achieved:

* **Accuracy:** 98.25%
* **Precision:** 98.61%
* **Recall:** 98.61%
* **F1-Score:** 98.61%
* **AUC:** 0.9954

Therefore, Logistic Regression was selected as the preferred model for this experiment.

## 📁 Project Structure

```text
maincrafts-ai-ml-task4-classification/
│
├── AI_Task4_Classification_Evaluation.ipynb
├── AI_Task4_Mandatory_Deliverables_Report.pdf
├── Task4_Confusion_Matrix.png
├── Task4_ROC_Curve.png
├── Task4_Model_Comparison.csv
└── README.md
```

## 📷 Results

### Confusion Matrix

The project includes the generated confusion matrix:

`Task4_Confusion_Matrix.png`

### ROC Curve

The ROC curve comparison is available in:

`Task4_ROC_Curve.png`

## 📄 Deliverables

* ✅ Jupyter Notebook
* ✅ Confusion Matrix
* ✅ Classification Report
* ✅ ROC Curve
* ✅ AUC Score
* ✅ Model Comparison
* ✅ Class Imbalance Handling
* ✅ Final Model Decision
* ✅ 2–3 Page PDF Report

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Open the project

Open the project folder in **Jupyter Notebook** or **JupyterLab**.

### 3. Open the notebook

```text
AI_Task4_Classification_Evaluation.ipynb
```

### 4. Run the cells

Execute the notebook cells from top to bottom.

## 👨‍💻 Author

**Harish V.**

B.E. Electronics and Communication Engineering
Artificial Intelligence & Machine Learning Internship – Maincrafts Technology

---

⭐ If you find this project useful, consider giving the repository a star!
