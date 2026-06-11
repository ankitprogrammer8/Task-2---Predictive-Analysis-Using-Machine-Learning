# 🤖 Task 2 — Predictive Analysis Using Machine Learning

**CodTech IT Solutions Pvt. Ltd. | Data Analytics Internship**

---

## 📋 Internship Details

| Field | Details |
|-------|---------|
| **Name** | Ankit Kumar Pradhan |
| **Company** | CODTECH IT Solutions Pvt. Ltd. |
| **Intern ID** | CITS442 |
| **Domain** | Data Analytics |
| **Duration** | 4 Weeks |
| **Mentor** | Neela Santhosh Kumar |

---

## 📌 Task Overview

Build a Machine Learning model (Classification) to predict student pass/fail outcomes based on academic and lifestyle features. The notebook covers feature selection, model training, and detailed evaluation.

---

## 📁 Project Structure

```
Task-2-Predictive-Analysis/
│
├── predictive_analysis_ml.ipynb   # Main Jupyter Notebook
├── student_performance.csv        # Dataset used for training & testing
└── README.md                      # Project documentation
```

---

## 📊 Dataset Description

**File:** `student_performance.csv`  
**Records:** 100 students | **Features:** 12 columns

| Column | Description |
|--------|-------------|
| StudentID | Unique student identifier |
| Age | Student age |
| Gender | Male / Female |
| StudyHoursPerDay | Daily study hours |
| AttendanceRate | Class attendance percentage |
| PreviousGrade | Grade from previous semester |
| ParentalEducation | Parent's education level |
| InternetAccess | Internet access at home (Yes/No) |
| ExtracurricularActivities | Participation in activities (Yes/No) |
| SleepHours | Average sleep hours per night |
| FinalGrade | Final exam grade |
| **Pass** | **Target: 1 = Pass, 0 = Fail** |

---

## 🔧 Steps Performed

### 1. 📥 Data Loading & Exploration
- Loaded CSV dataset using Pandas
- Explored shape, data types, and statistical summary
- Checked for missing values

### 2. 📈 Exploratory Data Analysis (EDA)
- Visualized target variable distribution (Pass vs Fail)
- Plotted study hours, attendance, and grade distributions
- Generated correlation heatmap

### 3. 🛠️ Data Preprocessing
- Encoded categorical columns (Gender, ParentalEducation, InternetAccess, ExtracurricularActivities) using LabelEncoder
- Applied StandardScaler for feature normalization

### 4. 🎯 Feature Selection
- Applied **SelectKBest** with ANOVA F-Test
- Identified top features: `StudyHoursPerDay`, `AttendanceRate`, `PreviousGrade`
- Visualized feature importance scores

### 5. 🤖 Model Training
- Split data: **80% train / 20% test** (stratified)
- Trained two models:
  - **Logistic Regression**
  - **Random Forest Classifier**

### 6. 📊 Model Evaluation
- Accuracy Score
- Classification Report (Precision, Recall, F1-Score)
- Confusion Matrix
- ROC Curve & AUC Score
- Feature Importance (Random Forest)

---

## 📦 Libraries Used

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Install all dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 🚀 How to Run

1. Clone or download this repository
2. Make sure `student_performance.csv` is in the same folder as the notebook
3. Open the notebook:
   ```bash
   jupyter notebook predictive_analysis_ml.ipynb
   ```
4. Run all cells from top to bottom (`Kernel > Restart & Run All`)

---

## 🏆 Results

| Model | Accuracy | AUC Score |
|-------|----------|-----------|
| Logistic Regression | ~95%+ | ~0.97+ |
| Random Forest | ~97%+ | ~0.99+ |

> **Best Model: Random Forest Classifier**

---

## 🔑 Key Findings

- **Study Hours Per Day** is the most important predictor of student success
- **Attendance Rate** and **Previous Grade** are also highly influential
- Students who study 4+ hours/day and attend 80%+ classes have very high pass rates
- Internet access and parental education have moderate influence

---

*Completion Certificate will be issued on Internship End Date.*
