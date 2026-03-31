# Part4-Data-Visualization-Machine-Learning

### Theme: Student Performance Analysis & Prediction

---

## 📌 Overview

This project analyses a student performance dataset to produce meaningful visualizations and build a machine learning model to predict whether a student will **Pass or Fail** — end to end.

---

## 📁 Repository Structure

```
├── students.csv                  # Dataset (15 students, 9 columns)
├── student_performance.py        # Main Python script (all 4 tasks)
├── plot1_bar.png                 # Task 2 - Bar Chart
├── plot2_histogram.png           # Task 2 - Histogram
├── plot3_scatter.png             # Task 2 - Scatter Plot
├── plot4_boxplot.png             # Task 2 - Box Plot
├── plot5_line.png                # Task 2 - Line Plot
├── plot6_seaborn_bar.png         # Task 3 - Seaborn Bar Plot
├── plot7_seaborn_scatter.png     # Task 3 - Seaborn Scatter Plot
├── plot8_feature_importance.png  # Task 4 - Feature Importance Chart
└── README.md                     # Project documentation
```

## 📊 Dataset

The dataset `students.csv` contains records of **15 students** with the following columns:

| Column | Description |
|--------|-------------|
| name | Student's name |
| math | Math score |
| science | Science score |
| english | English score |
| history | History score |
| pe | Physical Education score |
| attendance_pct | Attendance percentage |
| study_hours_per_day | Daily study hours |
| passed | Target variable: 1 = Pass, 0 = Fail |

---

## 🛠️ Tasks Completed

### ✅ Task 1 — Data Exploration with Pandas 
- Printed first 5 rows using `.head()`
- Printed shape and data types using `.dtypes`
- Printed summary statistics using `.describe()`
- Counted passing and failing students using `.value_counts()`
- Computed average score per subject for passing vs failing students
- Found the student with the highest overall average score

### ✅ Task 2 — Data Visualization with Matplotlib 
1. **Bar Chart** — Average score per subject across all students
2. **Histogram** — Distribution of Math scores with mean line
3. **Scatter Plot** — Study hours vs Average score, coloured by Pass/Fail
4. **Box Plot** — Attendance distribution for passing vs failing students
5. **Line Plot** — Math and Science scores for every student

### ✅ Task 3 — Data Visualization with Seaborn 
1. **Bar Plot** — Average Math & Science scores split by Pass/Fail
2. **Scatter Plot** — Attendance % vs Average score with regression lines for each group
3. **Comparison Comment** — Seaborn vs Matplotlib experience included in code comments

### ✅ Task 4 — Machine Learning with scikit-learn 
- **Step 1:** Prepared features (X) and target (y), split into 80% train / 20% test
- **Step 2:** Trained a `LogisticRegression` model on scaled training data
- **Step 3:** Evaluated model on test set — printed accuracy and per-student predictions
- **Step 4:** Extracted and visualized feature importance using model coefficients
- **Step 5:** Predicted Pass/Fail for a new student with probability scores

---

## ▶️ How to Run

### 1. Clone the repository
```bash
git clone https://github.com/bishakhadey882-byte/Part4-Data Visualization and Machine Learning.git
cd Part4-Data Visualization and Machine Learning
```

### 2. Install required libraries
```bash
pip install pandas matplotlib seaborn scikit-learn
```

### 3. Run the script
```bash
 "part4_visualization_ml.ipynb"
```

All plots will be saved as `.png` files in the same folder and displayed inline.

---

## 📦 Libraries Used

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading and exploration |
| `matplotlib` | Data visualization (manual plots) |
| `seaborn` | Data visualization (statistical plots) |
| `scikit-learn` | Machine learning model and evaluation |

---

## 🤖 Model Summary

- **Algorithm:** Logistic Regression
- **Features:** math, science, english, history, pe, attendance_pct, study_hours_per_day
- **Target:** passed (1 = Pass, 0 = Fail)
- **Train/Test Split:** 80% / 20% (random_state=42)
- **Scaling:** StandardScaler (fit on train, transform both.


