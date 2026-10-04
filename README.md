# 📊 Statistical Analysis and Hypothesis Testing in Python

## Week 3 — Data Science Project

## 📌 Project Overview

This project performs statistical analysis and hypothesis testing using Python to investigate the relationship between students' reported weekly study time and their final mathematics grades.

The analysis uses the **Student Performance dataset** from the UCI Machine Learning Repository. It applies statistical techniques to explore patterns, test hypotheses, compare group averages, and interpret the significance of observed relationships.

The project demonstrates the practical application of Python libraries for data cleaning, exploratory data analysis, statistical testing, visualization, and report generation.

## 🎯 Objectives

* Load and prepare a publicly available dataset.
* Perform exploratory data analysis and descriptive statistics.
* Formulate null and alternative hypotheses.
* Investigate the relationship between study-time categories and final grades.
* Perform Spearman rank correlation.
* Compare two study-time groups using Welch's independent-samples t-test.
* Compare multiple groups using one-way ANOVA.
* Perform simple linear regression.
* Interpret p-values, confidence intervals, and statistical significance.
* Generate visualizations and an automated Word report.

## 📂 Project Structure

```text
Week3_Hypothesis_Testing/
│
├── data/
│   └── student-mat.csv
│
├── visualizations/
│   ├── 01_grade_distribution.png
│   ├── 02_grades_by_studytime.png
│   ├── 03_average_grade.png
│   └── 04_studytime_grade_scatter.png
│
├── Week3_Statistical_Analysis.ipynb
├── Week3_Hypothesis_Testing_Report.docx
├── statistical_test_results.csv
└── README.md
```

## 📚 Dataset

**Source:** UCI Machine Learning Repository

**Dataset:** Student Performance — Mathematics

**Dataset link:**
https://archive.ics.uci.edu/dataset/320/student+performance

The analysis focuses on the following variables:

| Variable    | Description                                              |
| ----------- | -------------------------------------------------------- |
| `studytime` | Ordinal category representing reported weekly study time |
| `G3`        | Final mathematics grade on a scale from 0 to 20          |

The study-time variable has four categories, ranging from less than two hours per week to more than ten hours per week.

## 🔬 Research Question

Is there a statistically significant monotonic relationship between students' reported weekly study time and their final mathematics grades?

### Hypotheses

**Null Hypothesis (H₀):** There is no monotonic association between study time and final mathematics grades in the population.

**Alternative Hypothesis (H₁):** There is a monotonic association between study time and final mathematics grades in the population.

**Significance Level:** α = 0.05

## 🧪 Statistical Methods

### 1. Spearman Rank Correlation

Evaluates the direction and strength of the monotonic association between study-time categories and final mathematics grades.

### 2. Welch's Independent-Samples t-Test

Compares the mean final grades of students in lower study-time categories (1–2) with those in higher study-time categories (3–4), without assuming equal population variances.

### 3. One-Way ANOVA

Examines whether mean final grades differ across the four study-time categories.

### 4. Linear Regression

Summarizes the linear relationship between the numerical coding of study-time categories and final mathematics grades.

## 📈 Visualizations

The project generates the following charts:

1. **Grade Distribution:** Displays the distribution of final mathematics grades.
2. **Grades by Study Time:** Compares grade distributions across study-time categories using a box plot.
3. **Average Grade by Study Time:** Visualizes the mean final grade for each category.
4. **Individual Grade Comparison:** Shows individual student grades across study-time categories.

All charts are saved in the `visualizations/` directory and can be included in the final report.

## 🛠️ Technologies Used

* **Python** — Programming language
* **Pandas** — Data manipulation and preparation
* **NumPy** — Numerical computing
* **SciPy** — Statistical hypothesis testing
* **Statsmodels** — Regression and confidence intervals
* **Matplotlib** — Data visualization
* **Seaborn** — Statistical visualization
* **Jupyter Notebook** — Interactive analysis
* **python-docx** — Automated Word report generation

## ⚙️ Installation and Setup

### Prerequisites

* Python 3.10 or later recommended
* Visual Studio Code
* Python and Jupyter extensions for VS Code

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd Week3_Hypothesis_Testing
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

Alternatively, download the project ZIP file and extract it.

### Step 2: Install dependencies

Open a terminal in the project directory and run:

```bash
python -m pip install pandas numpy scipy statsmodels matplotlib seaborn jupyter ipykernel python-docx
```

On Windows, if `python` is not recognized, try using `py` instead.

### Step 3: Download the dataset

Download the Student Performance dataset from:

https://archive.ics.uci.edu/dataset/320/student+performance

Extract the archive and place `student-mat.csv` inside the `data/` folder.

The expected path is:

```text
data/student-mat.csv
```

### Step 4: Open the notebook

Open `Week3_Statistical_Analysis.ipynb` in VS Code or Jupyter Notebook.

Select the installed Python environment as the kernel.

### Step 5: Execute the analysis

Run the notebook cells in order, starting from the imports and dataset loading.

The notebook performs data preparation, creates visualizations, executes statistical tests, and generates the statistical results summary.

### Step 6: Generate the Word report

Run the report-generation cell in the notebook after executing all prerequisite analysis cells.

The generated report is saved as:

```text
Week3_Hypothesis_Testing_Report.docx
```

## 📊 Interpreting the Results

The analysis uses a significance level of 0.05.

* If a test's p-value is below 0.05, its corresponding null hypothesis is rejected.
* If the p-value is 0.05 or higher, the null hypothesis is not rejected.
* Correlation coefficients indicate the direction and strength of an association.
* Confidence intervals communicate the uncertainty around estimated quantities.

The final conclusions should be based on the actual output generated by the notebook rather than assumed or predetermined results.

## ⚠️ Limitations

* The dataset is observational and does not establish causation.
* Study time is reported in broad categories rather than exact hours.
* Academic performance may be influenced by many other factors.
* Statistical tests have assumptions that should be checked before drawing conclusions.
* Results from this dataset may not generalize to all student populations.

## 📄 Project Deliverables

* Executable Jupyter Notebook containing Python code and analysis outputs.
* Four statistical visualizations.
* CSV file containing the statistical test results.
* Word report documenting the methodology, findings, and conclusions.
* README file containing project documentation and setup instructions.

## 🎓 Conclusion

This project demonstrates how Python can be used to investigate a real-world research question through descriptive statistics, visualization, hypothesis testing, and regression analysis.

By combining multiple statistical techniques, the project provides a structured approach to examining the association between reported study habits and academic performance. It also emphasizes the importance of interpreting statistical significance alongside effect estimates, confidence intervals, assumptions, and research limitations.

## 📚 References

1. UCI Machine Learning Repository — Student Performance Dataset: https://archive.ics.uci.edu/dataset/320/student+performance
2. SciPy Documentation: https://docs.scipy.org/doc/scipy/
3. Pandas Documentation: https://pandas.pydata.org/docs/
4. Statsmodels Documentation: https://www.statsmodels.org/
5. Matplotlib Documentation: https://matplotlib.org/stable/
6. Seaborn Documentation: https://seaborn.pydata.org/
