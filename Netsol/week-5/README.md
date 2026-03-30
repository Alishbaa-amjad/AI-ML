# 📊 Titanic Dataset - Statistical Distribution Analysis

## 📌 Project Overview

This project focuses on analyzing the **Titanic dataset** using different **statistical distributions** and **data visualization techniques**. The main goal is to understand how different types of data behave and how appropriate distributions can be applied to each column.

---

## 🎯 Objectives

* Explore dataset and understand column types
* Apply different probability distributions
* Visualize data using graphs
* Check normality of numerical data
* Apply transformations (log, z-score) to improve distribution

---

## 📂 Dataset

The dataset used in this project contains the following columns:

* PassengerId
* Survived
* Pclass
* Name
* Sex
* Age
* SibSp
* Parch
* Ticket
* Fare
* Cabin
* Embarked

---

## 📊 Distributions Applied

| Distribution       | Column Used            | Reason                               |
| ------------------ | ---------------------- | ------------------------------------ |
| **Bernoulli**      | Survived, Sex (binary) | Binary outcomes (0/1)                |
| **Binomial**       | Survived               | Multiple Bernoulli trials            |
| **Poisson**        | SibSp, Parch           | Count data                           |
| **Exponential**    | Fare                   | Continuous & right-skewed            |
| **Normal**         | Age                    | Continuous & approximately symmetric |
| **t-Distribution** | Age (sample)           | Small sample analysis                |

---

## 📈 Visualizations Used

* Histogram + KDE
* Boxplot (outliers detection)
* Countplot (categorical data)
* Pie chart
* Probability plots

---

## 🔄 Data Transformation

To improve normality:

* **Log Transformation**

  * Applied on: `Fare`
  * Result: Reduced skewness and improved symmetry

* **Z-score Normalization**

  * Applied on: `Age`
  * Result: Standardized data (mean = 0, std = 1)

---

## 🧪 Normality Testing

* Used **Shapiro-Wilk Test**
* Decision rule:

  * p-value > 0.05 → Data is Normal
  * p-value < 0.05 → Data is Not Normal

---

## 🔍 Key Insights

* `Fare` is highly right-skewed → behaves like exponential distribution
* `Age` is approximately normally distributed
* `SibSp` and `Parch` follow count-based (Poisson-like) behavior
* Categorical variables require frequency-based visualization

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy

---

## ▶️ How to Run

1. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scipy
```

2. Run the notebook or Python file:

```bash
python analysis.py
```

---

## 📌 Conclusion

This project demonstrates how different statistical distributions can be applied based on data type. It also shows how transformations help in achieving normality, which is important for many statistical methods.

---

## 🙌 Author

**Alishba Amjad**
BS Computer Science (Final Semester)

---

## ⭐ Acknowledgment

This project was completed as part of a university assignment to understand **data distributions and statistical analysis**.

---

