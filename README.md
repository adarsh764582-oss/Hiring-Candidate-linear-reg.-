# Salary Prediction using Linear Regression

This project demonstrates how to build a **salary prediction model** using **Linear Regression** in Python.  
The model predicts an employee’s salary based on:

- Years of experience
- Test score (out of 10)
- Interview score (out of 10)

The dataset includes missing values and text-based data, which are cleaned and transformed before training the model.

---

## 📂 Dataset

**File:** `hiring.csv`

**Columns:**
- `experience` – Years of experience (given as words like *two, five, seven*)
- `test_score(out of 10)` – Candidate’s test score
- `interview_score(out of 10)` – Candidate’s interview score
- `salary($)` – Salary (target variable)

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- word2number
- Jupyter Notebook

---

## 🔄 Data Preprocessing

1. **Missing Values**
   - `experience`: Filled with `"zero"`
   - `test_score(out of 10)`: Filled with the floor value of the mean test score

2. **Text to Numeric Conversion**
   - Converted experience values from words to numbers using `word2number`

Example:
"five" → 5
"zero" → 0


---

## 📈 Model Used

- **Linear Regression** (`sklearn.linear_model.LinearRegression`)

**Features:**
- Experience
- Test Score
- Interview Score

**Target:**
- Salary

---
