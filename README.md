# 📊 Matplotlib — Zero to Advanced for AI/ML QA Engineers

### 🎨 Complete Python Data Visualization Guide | Beginner to Advanced

<p align="center">
  <a href="https://github.com/kunchinareshkumar/datavisualization-matplotlib-aiml-python/blob/main/Matplotlib_Zero_to_Advanced_AI_ML_QA.ipynb">
    <img src="https://img.shields.io/badge/📘_Open-Jupyter_Notebook-blue?style=for-the-badge" alt="Open Notebook"/>
  </a>
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Matplotlib-Data_Visualization-orange?style=for-the-badge" alt="Matplotlib"/>
  <img src="https://img.shields.io/badge/Focus-AI%2FML_QA-green?style=for-the-badge" alt="AI ML QA"/>
  <img src="https://img.shields.io/badge/Level-Zero_to_Advanced-purple?style=for-the-badge" alt="Zero to Advanced"/>
</p>

---

## 📌 About This Repository

Welcome to the **Matplotlib Zero-to-Advanced Learning Repository**! 🚀

This repository is designed to help Python learners, QA Engineers, SDETs, aspiring AI/ML testers, and data science enthusiasts master data visualization using Matplotlib through practical Python examples.

The goal is to understand not only **how to create charts**, but also how to interpret visual patterns, analyze data quality, investigate anomalies, and evaluate machine learning model behavior.

Whether you are starting with Python or preparing for AI/ML testing, this notebook provides a structured learning resource for building your visualization skills.

## 🎯 Learning Objectives

- 📈 Understand Matplotlib fundamentals and its architecture.
- 📊 Learn common and advanced chart types.
- 🎨 Customize charts using titles, labels, colors, legends, grids, and annotations.
- 🧩 Work with multiple plots, subplots, and layouts.
- 🔍 Apply visualization techniques to exploratory data analysis (EDA).
- 🧪 Visualize test results, defects, failures, and performance metrics.
- 🤖 Understand how visualization supports ML model evaluation and monitoring.
- 💼 Build practical skills relevant to QA, SDET, AI/ML testing, and data testing.

## 📚 Table of Contents

1. [Introduction to Matplotlib](#-1-introduction-to-matplotlib)
2. [Installation and Setup](#-2-installation-and-setup)
3. [Matplotlib Architecture](#-3-matplotlib-architecture)
4. [Basic Plotting Concepts](#-4-basic-plotting-concepts)
5. [Essential Chart Types](#-5-essential-chart-types)
6. [Chart Customization](#-6-chart-customization)
7. [Advanced Visualization](#-7-advanced-visualization)
8. [NumPy and Pandas Integration](#-8-numpy-and-pandas-integration)
9. [EDA and Data Quality Testing](#-9-eda-and-data-quality-testing)
10. [AI/ML Testing Applications](#-10-aiml-testing-applications)
11. [QA Automation Visualization](#-11-qa-automation-visualization)
12. [Best Practices](#-12-best-practices)
13. [Practice Projects](#-13-practice-projects)
14. [Interview Preparation](#-14-interview-preparation)
15. [How to Run the Notebook](#-15-how-to-run-the-notebook)
16. [Learning Roadmap](#-16-learning-roadmap)
17. [References](#-17-references)

---

## 📘 1. Introduction to Matplotlib

**Matplotlib** is a Python library used to create static, animated, and interactive visualizations.

It helps convert numerical and categorical data into charts that make trends, distributions, relationships, and anomalies easier to understand.

### Why learn Matplotlib?

| Use Case | Example |
|---|---|
| Data analysis | Explore customer or sales data |
| Data quality | Identify missing values and unusual distributions |
| QA testing | Visualize test pass/fail trends |
| Performance testing | Compare response times and throughput |
| Machine learning | Plot training and validation loss |
| Model evaluation | Visualize confusion matrices and ROC curves |
| Monitoring | Observe metric changes and potential drift |

## 🛠️ 2. Installation and Setup

Install the required libraries:

```bash
python3 -m pip install matplotlib numpy pandas jupyter
```

Import the libraries:

```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
```

Create your first plot:

```python
x = [1, 2, 3, 4, 5]
y = [10, 20, 15, 30, 25]

plt.plot(x, y, marker="o")
plt.title("My First Matplotlib Plot")
plt.xlabel("X Values")
plt.ylabel("Y Values")
plt.grid(True)
plt.show()
```

## 🏗️ 3. Matplotlib Architecture

Understand the core components before exploring chart types.

| Component | Purpose |
|---|---|
| Figure | The complete figure or canvas |
| Axes | The individual plotting area |
| Axis | Controls coordinates, ticks, and scale |
| Artists | Visual elements such as lines, text, and patches |
| Title | Describes the chart |
| Labels | Explain the X and Y axes |
| Legend | Identifies plotted data series |
| Grid | Helps compare values |
| Ticks | Show coordinate reference values |

Recommended object-oriented approach:

```python
fig, ax = plt.subplots(figsize=(8, 5))

ax.plot([1, 2, 3], [10, 20, 15], marker="o")
ax.set_title("Sales Trend")
ax.set_xlabel("Month")
ax.set_ylabel("Sales")

plt.show()
```

## 📈 4. Basic Plotting Concepts

Learn these fundamentals:

- `plt.figure()` — create a figure.
- `plt.subplots()` — create figures and axes.
- `plt.plot()` — draw line plots.
- `plt.show()` — display plots.
- `plt.savefig()` — save plots.
- `plt.close()` — close figures.
- `plt.title()` — add a title.
- `plt.xlabel()` and `plt.ylabel()` — label axes.
- `plt.legend()` — display a legend.
- `plt.grid()` — display a grid.
- `plt.xlim()` and `plt.ylim()` — control axis limits.

## 📊 5. Essential Chart Types

| Chart | Matplotlib Function | Common Application |
|---|---|---|
| Line plot | `plt.plot()` | Trends over time |
| Bar chart | `plt.bar()` | Compare categories |
| Horizontal bar | `plt.barh()` | Compare ranked categories |
| Scatter plot | `plt.scatter()` | Relationships between variables |
| Histogram | `plt.hist()` | Data distribution |
| Pie chart | `plt.pie()` | Parts of a whole |
| Box plot | `plt.boxplot()` | Spread and potential outliers |
| Area plot | `plt.fill_between()` | Magnitude and cumulative trends |
| Stacked bar | `plt.bar(..., bottom=...)` | Category composition |
| Error bar | `plt.errorbar()` | Uncertainty and variation |
| Heatmap | `plt.imshow()` | Matrix and correlation patterns |
| Contour plot | `plt.contour()` | Levels of a continuous function |
| 3D plot | `ax.plot_surface()` | Three-dimensional relationships |

## 🎨 6. Chart Customization

Make visualizations readable and informative.

Topics to practice:

- Colors and color maps
- Markers and line styles
- Figure size and resolution
- Titles and axis labels
- Legends and grid styling
- Font size and font weight
- Axis limits and tick formatting
- Annotations and text
- Transparency using `alpha`
- Multiple lines on a chart
- Saving charts as PNG, PDF, or SVG
- Layout management using `tight_layout()` or constrained layout

Example:

```python
months = ["Jan", "Feb", "Mar", "Apr"]
sales = [100, 150, 130, 200]

fig, ax = plt.subplots(figsize=(8, 5))

ax.bar(months, sales, color="skyblue")
ax.set_title("Monthly Sales")
ax.set_xlabel("Month")
ax.set_ylabel("Sales")
ax.grid(axis="y", alpha=0.3)

plt.tight_layout()
plt.show()
```

## 🚀 7. Advanced Visualization

Explore these concepts after mastering the basics:

- Multiple subplots
- Shared X and Y axes
- Twin axes
- Secondary scales
- Logarithmic scales
- Error bars and uncertainty
- Annotations and callouts
- Custom tick formatters
- Color bars
- Heatmaps
- Contour and filled contour plots
- Three-dimensional charts
- Animations
- Plot styles and `rcParams`
- Figure export and resolution
- Reusable visualization functions

## 🔗 8. NumPy and Pandas Integration

Matplotlib works naturally with NumPy arrays and Pandas DataFrames.

### NumPy example

```python
x = np.arange(1, 6)
y = x ** 2

plt.plot(x, y, marker="o")
plt.title("Square Values")
plt.show()
```

### Pandas example

```python
df = pd.DataFrame({
    "Month": ["Jan", "Feb", "Mar", "Apr"],
    "Sales": [100, 150, 130, 200]
})

df.plot(x="Month", y="Sales", kind="bar")
plt.tight_layout()
plt.show()
```

Practice visualizing CSV data, distributions, grouped results, missing values, and outliers.

## 🔍 9. EDA and Data Quality Testing

Exploratory Data Analysis (EDA) helps uncover patterns and data-quality problems before model training or application decisions.

| Quality Check | Visualization |
|---|---|
| Feature distribution | Histogram |
| Potential outliers | Box plot |
| Relationship between features | Scatter plot |
| Correlation patterns | Heatmap |
| Category imbalance | Bar chart |
| Time-dependent changes | Line plot |
| Data before and after cleaning | Comparative plots |
| Dataset or feature drift | Distribution comparison |

**Important:** A chart can reveal suspicious patterns, but it does not independently prove a data-quality defect. Confirm findings with data checks, statistical tests, and business rules.

## 🤖 10. AI/ML Testing Applications

Matplotlib is useful for investigating model performance and supporting AI/ML quality assurance.

| Testing Area | What to Visualize |
|---|---|
| Model validation | Training and validation metrics |
| Overfitting | Training versus validation loss |
| Classification testing | Confusion matrix |
| Model comparison | Accuracy, precision, recall, and F1 |
| Threshold analysis | Precision-recall and ROC curves |
| Regression testing | Actual versus predicted values |
| Error analysis | Residual distributions |
| Data drift | Reference versus current distributions |
| Model monitoring | Metric changes over time |
| Fairness analysis | Performance across relevant groups |

These visualizations support investigation; they do not replace quantitative evaluation, acceptance criteria, or dedicated statistical tests.

## 🧪 11. QA Automation Visualization

Visualize automated testing results to improve reporting and debugging.

Possible applications include:

- Test execution trends
- Pass, fail, and skipped test counts
- Defect trends across releases
- API response-time distributions
- Performance-test throughput
- Failure rates across browsers
- Regression results across builds
- Flaky test frequency
- Model evaluation results across versions

Example:

```python
import matplotlib.pyplot as plt

results = {
    "Passed": 85,
    "Failed": 10,
    "Skipped": 5
}

plt.bar(results.keys(), results.values())
plt.title("Automated Test Execution Summary")
plt.xlabel("Test Status")
plt.ylabel("Number of Tests")
plt.show()
```

## ✅ 12. Best Practices

- Select a chart that matches the question being investigated.
- Use clear titles, axis labels, units, and legends.
- Avoid misleading scales and unnecessary visual decoration.
- Choose accessible colors and distinguishable markers.
- Use reproducible datasets and clearly defined metrics.
- Check missing values and data types before plotting.
- Validate calculations behind plotted metrics.
- Label uncertainty and sample sizes when relevant.
- Save important figures with suitable resolution.
- Use the object-oriented Matplotlib API for reusable code.

## 💡 13. Practice Projects

Try these projects to reinforce your learning.

| Project | Skills Practiced |
|---|---|
| 1. Student marks analysis | Line, bar, and histogram plots |
| 2. Customer dataset EDA | Pandas, distributions, box plots |
| 3. API performance report | Response-time distributions and trends |
| 4. Automation test dashboard | Pass/fail metrics and defect trends |
| 5. ML model evaluation | Confusion matrix and ROC visualization |
| 6. Data drift investigation | Distribution comparisons |
| 7. Model monitoring report | Metrics over time |
| 8. Release quality report | Regression trends and test outcomes |

## 🎤 14. Interview Preparation

Prepare to explain:

1. What is Matplotlib, and why is it useful?
2. What is the difference between Figure, Axes, and Axis?
3. When would you use a histogram instead of a bar chart?
4. How can a box plot help identify outliers?
5. How do you create multiple subplots?
6. How do you plot data from CSV files using Pandas?
7. How can you visualize model overfitting?
8. How would you compare model performance across versions?
9. How can visualization support data-drift investigation?
10. How would you visualize automated test execution results?

## ▶️ 15. How to Run the Notebook

**Option 1 — Open directly on GitHub**

[Open Matplotlib Zero-to-Advanced AI/ML QA Notebook](https://github.com/kunchinareshkumar/datavisualization-matplotlib-aiml-python/blob/main/Matplotlib_Zero_to_Advanced_AI_ML_QA.ipynb)

**Option 2 — Run locally on macOS**

Clone the repository and enter its folder:

```bash
git clone https://github.com/kunchinareshkumar/datavisualization-matplotlib-aiml-python.git

cd datavisualization-matplotlib-aiml-python
```

Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the dependencies and start Jupyter:

```bash
python -m pip install matplotlib numpy pandas jupyter
python -m jupyter notebook
```

Open `Matplotlib_Zero_to_Advanced_AI_ML_QA.ipynb` and execute the notebook cells in sequence.

## 🗺️ 16. Learning Roadmap

| Stage | Learning Focus |
|---|---|
| Beginner | Setup, architecture, basic plots |
| Intermediate | Chart types, labels, customization |
| Advanced | Subplots, heatmaps, annotations, 3D |
| Data Analysis | Pandas integration and EDA |
| QA Applications | Test reports and performance metrics |
| AI/ML Applications | Model evaluation and drift visualization |
| Portfolio | Complete practical visualization projects |

## 📚 17. References

- [Official Matplotlib Documentation](https://matplotlib.org/stable/)
- [Matplotlib Tutorials](https://matplotlib.org/stable/tutorials/)
- [Matplotlib Gallery](https://matplotlib.org/stable/gallery/)
- [NumPy Documentation](https://numpy.org/doc/)
- [Pandas Visualization Guide](https://pandas.pydata.org/docs/user_guide/visualization.html)

---

## 🌟 Who Is This Repository For?

- Python beginners learning data visualization
- QA Engineers and SDETs expanding their technical skills
- Automation Engineers creating visual test reports
- AI/ML Test Engineers learning model evaluation
- Data QA Engineers exploring EDA and data quality
- Aspiring data science and machine learning professionals

## 🤝 Contributions

Suggestions, corrections, and improvements are welcome. Feel free to open an issue or submit a pull request to help improve this learning resource.

## 👨‍💻 Author

**Naresh Kumar**

Learning and sharing practical resources in Python, data visualization, QA automation, and AI/ML testing.

---

⭐ **If you find this repository useful, consider giving it a star and sharing it with other learners!**

*Learn → Practice → Visualize → Test → Improve*
