# 🫁 Lung Cancer Detection

A machine learning project for predicting the presence of **lung cancer** based on a set of patient-reported symptoms and lifestyle-related features.

The project uses supervised machine learning to analyze health-related attributes such as coughing, wheezing, chest pain, fatigue, alcohol consumption, and chronic disease to classify whether a patient is likely to have lung cancer.

> **Model Accuracy: 89.29%**

---

## 📌 Project Overview

Lung cancer is one of the leading causes of cancer-related deaths worldwide. Early identification of potential risk factors can help support further medical investigation.

This project explores how machine learning can be applied to structured patient data to predict the `LUNG_CANCER` target variable.

### 🎯 Objective

Build a classification model that predicts:

* `YES` → Lung cancer detected
* `NO` → Lung cancer not detected

The model is trained using symptoms, lifestyle factors, and medical-history-related features.

> ⚠️ **Disclaimer:** This project is intended for educational and research purposes only. It is not a medical diagnostic system and should not be used as a substitute for professional medical advice.

---

## 🧠 Machine Learning Workflow

```text
Patient Dataset
      │
      ▼
Data Exploration
      │
      ▼
Data Preprocessing
      │
      ▼
Feature Selection
      │
      ▼
Train / Test Split
      │
      ▼
Machine Learning Model
      │
      ▼
Prediction
      │
      ▼
Model Evaluation
      │
      ├── Accuracy
      └── Confusion Matrix
```

---

## 📊 Features

The dataset contains the following attributes:

| Feature                 | Description                 |
| ----------------------- | --------------------------- |
| `PEER_PRESSURE`         | Influence from peers        |
| `CHRONIC DISEASE`       | Presence of chronic disease |
| `FATIGUE`               | Presence of fatigue         |
| `ALLERGY`               | Presence of allergies       |
| `WHEEZING`              | Presence of wheezing        |
| `ALCOHOL CONSUMING`     | Alcohol consumption         |
| `COUGHING`              | Presence of coughing        |
| `SWALLOWING DIFFICULTY` | Difficulty swallowing       |
| `CHEST PAIN`            | Presence of chest pain      |
| `ANIXV`                 | Dataset-specific feature    |
| `LUNG_CANCER`           | Target variable             |

### Target Variable

```text
LUNG_CANCER
```

The target represents whether lung cancer is present in the given sample.

---

## 📈 Model Performance

The model achieved an accuracy of:

### **89.29% Accuracy**

```text
Accuracy = 0.8928571428571429
```

### Confusion Matrix

```text
[[ 7  5]
 [ 1 43]]
```

Visual representation:

```text
                 Predicted
               Negative  Positive
Actual Negative    7        5
       Positive    1       43
```

This means:

* **7** → Correctly classified negative cases
* **43** → Correctly classified positive cases
* **5** → Negative cases incorrectly classified as positive
* **1** → Positive case incorrectly classified as negative

---

## 🔍 Understanding the Results

The model correctly classified **50 out of 56 test samples**.

```text
Correct Predictions = 7 + 43 = 50

Total Samples = 56

Accuracy = 50 / 56
         ≈ 89.29%
```

The confusion matrix also shows that the model performed particularly well on the positive class, correctly identifying **43 cases**.

However, accuracy alone is not sufficient for evaluating a medical classification problem. Metrics such as **precision, recall, F1-score, and ROC-AUC** should also be considered.

---

## 🛠️ Technologies Used

* 🐍 Python
* 🧮 NumPy
* 🐼 Pandas
* 📊 Matplotlib
* 📈 Seaborn
* 🤖 Scikit-learn
* 📓 Jupyter Notebook

---

## 📂 Project Structure

```text
Lung-Cancer-Detection/
│
├── 📁 dataset/
│   └── lung_cancer.csv
│
├── 📓 Lung_Cancer_Detection.ipynb
│
├── 📄 README.md
│
└── 📄 requirements.txt
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Lung-Cancer-Detection.git
```

### 2. Navigate to the Project

```bash
cd Lung-Cancer-Detection
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
Lung_Cancer_Detection.ipynb
```

---

## 🧪 Model Evaluation

The model can be evaluated using multiple classification metrics:

```text
Accuracy
Precision
Recall
F1-Score
Confusion Matrix
ROC-AUC
```

For a medical prediction problem, **recall/sensitivity is particularly important**, because incorrectly classifying a positive cancer case as negative can have serious consequences.

---

## 💡 Key Learning Outcomes

This project demonstrates practical understanding of:

* Data preprocessing
* Exploratory Data Analysis
* Feature selection
* Binary classification
* Model training
* Model prediction
* Confusion matrix interpretation
* Classification evaluation metrics
* Applying machine learning to healthcare-related datasets

---

## 🔮 Future Improvements

Possible improvements include:

* [ ] Compare multiple classification algorithms
* [ ] Perform hyperparameter tuning
* [ ] Apply cross-validation
* [ ] Handle class imbalance
* [ ] Perform feature importance analysis
* [ ] Add precision, recall and F1-score
* [ ] Generate ROC-AUC curve
* [ ] Add SHAP-based model explainability
* [ ] Build an interactive prediction interface
* [ ] Deploy the model as a REST API
* [ ] Create a web-based prediction dashboard

---

## 📌 Conclusion

This project demonstrates how machine learning can be used to identify patterns in patient-related data and perform binary classification for lung cancer prediction.

With an achieved accuracy of **89.29%**, the model provides a strong baseline for further experimentation and improvement.

The project can be extended into a complete ML application by adding explainability, model comparison, an API layer, and an interactive frontend.

---

## ⭐ If You Find This Project Useful

Consider giving the repository a ⭐ and exploring the project!

**Built with Python & Machine Learning 🐍🤖**
