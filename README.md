# 🏦 Bank Customer Churn Analysis & Prediction

## Exploratory Data Analysis, Customer Behavior & Logistic Regression

**Bank Churners EDA** is a **Data Science and Machine Learning project focused on understanding customer churn in the banking sector**.

The project combines **Exploratory Data Analysis (EDA), statistical analysis, data visualization, customer segmentation, and Logistic Regression** to investigate the factors associated with customer attrition and build a foundation for predicting whether a banking customer is likely to leave.

The objective is not only to determine **who is churning**, but also to understand **why customers churn** and which behavioral, demographic, and financial characteristics can provide useful signals for customer retention strategies.

---

# 🎯 Business Problem

Customer churn represents a significant challenge for financial institutions.

When a customer leaves a bank, the institution loses:

* Existing revenue
* Future transaction opportunities
* Cross-selling potential
* Customer lifetime value
* Opportunities to build long-term relationships

A data-driven churn analysis can help answer questions such as:

> **Which customers are more likely to leave, and what characteristics distinguish them from retained customers?**

This project approaches the problem from two complementary perspectives:

```text
                BANK CUSTOMER DATA
                        │
            ┌───────────┴───────────┐
            │                       │
            ▼                       ▼
       DATA ANALYSIS          PREDICTIVE MODEL
            │                       │
            ▼                       ▼
     Customer Behavior       Logistic Regression
            │                       │
            └───────────┬───────────┘
                        ▼
               CHURN INSIGHTS
                        │
                        ▼
             RETENTION STRATEGIES
```

---

# 📊 Project Objectives

The project focuses on several key objectives:

* Understand the structure and quality of the banking dataset
* Explore customer demographics and financial characteristics
* Analyze the distribution of existing vs. attrited customers
* Identify patterns associated with customer churn
* Compare customer behavior across churn groups
* Analyze relationships between demographic and financial variables
* Investigate customer engagement and transaction behavior
* Perform statistical hypothesis testing
* Build a Logistic Regression classification model
* Establish a foundation for data-driven customer retention

---

# 🧠 Analytical Approach

The project follows a complete analytical workflow:

```text
Raw Dataset
     │
     ▼
Data Understanding
     │
     ▼
Data Cleaning & Inspection
     │
     ▼
Exploratory Data Analysis
     │
     ├── Numerical Analysis
     ├── Categorical Analysis
     ├── Distribution Analysis
     ├── Churn Segmentation
     └── Visualization
     │
     ▼
Statistical Analysis
     │
     ▼
Feature Preparation
     │
     ▼
Logistic Regression
     │
     ▼
Customer Churn Analysis
```

This workflow combines **descriptive analytics** with **predictive modeling**.

---

# 🔎 Exploratory Data Analysis

The EDA component investigates the structure and behavior of the customer population.

The analysis covers:

### Dataset Structure

Inspection of:

* Number of observations
* Number of variables
* Data types
* Missing values
* Numerical features
* Categorical features
* Distribution of the target variable

### Customer Demographics

The analysis explores variables such as:

* Customer age
* Gender
* Education level
* Income category
* Marital status
* Number of dependents

### Banking Behavior

The project also analyzes customer behavior through variables such as:

* Months on book
* Total relationship count
* Months inactive
* Contacts with the bank
* Credit limit
* Transaction amount
* Transaction count
* Credit utilization

These variables provide a behavioral view of customer engagement.

---

# 📈 Churn Analysis

The central target of the project is **customer attrition**.

The dataset distinguishes between customers who remain with the bank and customers who have left.

The analysis therefore compares:

```text
Existing Customers
        VS
Attrited Customers
```

across multiple dimensions.

---

## 👤 Customer Age

Age distributions are compared between retained and attrited customers to investigate whether customer lifecycle characteristics are associated with churn.

The analysis uses distribution visualizations and statistical testing to determine whether observed differences are statistically meaningful rather than simply visual differences.

---

## ⚧️ Gender Analysis

Customer churn is also examined across gender categories.

This allows the analysis to investigate whether the distribution of attrition differs between male and female customers.

---

## 💰 Income Category

Income segmentation provides another perspective on customer churn.

The project examines how attrition is distributed across different income categories and whether specific income groups demonstrate different customer behavior.

---

## 💳 Credit Limit

Credit-limit distributions are compared between existing and attrited customers.

This helps investigate whether financial capacity and credit-card characteristics are associated with customer retention.

---

## 💸 Transaction Behavior

Transaction activity provides one of the most important behavioral dimensions of the analysis.

The project examines:

* Total transaction amount
* Total transaction count
* Average utilization ratio

These variables help evaluate the relationship between **customer engagement and churn**.

---

# 📊 Visualization

The EDA notebooks use visual analysis to make customer behavior easier to interpret.

The project explores relationships using techniques such as:

* Distribution plots
* Bar charts
* Box plots
* Comparative visualizations
* Categorical analysis
* Numerical summaries

The objective is to move beyond raw statistics and identify **patterns that can be communicated to business stakeholders**.

---

# 🧪 Statistical Analysis

The project goes beyond descriptive statistics by applying hypothesis testing to selected customer characteristics.

A key example is testing whether customer age differs significantly between retained and attrited customers.

### Hypothesis Framework

```text
H₀:
No statistically significant difference exists
between the compared customer groups.

H₁:
A statistically significant difference exists
between the compared customer groups.
```

Statistical testing helps distinguish between:

```text
Observed Difference
        ≠
Statistically Significant Difference
```

This is an important principle in practical data analysis because visual differences alone do not necessarily imply meaningful relationships.

---

# 🤖 Logistic Regression

The repository also includes a dedicated **Logistic Regression notebook** for churn classification.

Logistic Regression is particularly suitable for this problem because the target represents a binary customer outcome:

```text
Customer
   │
   ├── Existing Customer
   │
   └── Attrited Customer
```

The model estimates the probability that a customer belongs to the churn class based on the available customer characteristics.

Conceptually:

```text
Customer Features
       │
       ▼
Data Preparation
       │
       ▼
Logistic Regression
       │
       ▼
Churn Probability
       │
       ├── Low Risk
       │
       └── Higher Risk
```

This provides a transition from **descriptive analytics** to **predictive analytics**.

---

# 🧮 Why Logistic Regression?

Logistic Regression is a strong baseline model for customer churn because it provides:

### Binary Classification

The model naturally handles two possible outcomes:

```text
0 → Existing Customer
1 → Attrited Customer
```

### Probability-Based Predictions

Rather than only returning a class, Logistic Regression can estimate the probability of churn.

### Interpretability

The model is easier to interpret than many black-box models, making it particularly useful in business environments where understanding the factors influencing predictions matters.

### Strong Baseline

Logistic Regression provides a useful benchmark before experimenting with more complex machine-learning algorithms.

---

# 🏗️ Machine Learning Pipeline

The predictive workflow can be summarized as:

```text
Customer Dataset
       │
       ▼
Data Preparation
       │
       ▼
Feature Selection
       │
       ▼
Feature Transformation
       │
       ▼
Train / Test Split
       │
       ▼
Logistic Regression
       │
       ▼
Predictions
       │
       ▼
Model Evaluation
```

The approach provides a foundation that can later be extended with additional classification algorithms.

---

# 💼 Business Perspective

The analytical findings can support several banking use cases.

### 🎯 Customer Retention

Identify customer segments that demonstrate behavioral characteristics associated with attrition.

### 📞 Targeted Outreach

Use churn-risk information to prioritize customer engagement campaigns.

### 💳 Product Strategy

Analyze whether customer product usage and transaction behavior are associated with retention.

### 📊 Customer Segmentation

Segment customers based on demographics, engagement, financial characteristics, and activity.

### 💰 Revenue Protection

Early identification of potentially departing customers can support proactive retention strategies.

---

# 🔬 Key Analytical Dimensions

The project analyzes churn through multiple dimensions rather than relying on a single feature.

| Dimension             | Examples                              |
| --------------------- | ------------------------------------- |
| 👤 Demographics       | Age, Gender, Education                |
| 💰 Financial          | Credit Limit, Income Category         |
| 💳 Engagement         | Transaction Count, Transaction Amount |
| ⏱️ Customer Lifecycle | Months on Book                        |
| 📞 Interaction        | Contacts with Bank                    |
| 💤 Activity           | Months Inactive                       |
| 📊 Credit Usage       | Average Utilization Ratio             |
| 🏦 Relationship       | Total Relationship Count              |

This multidimensional approach provides a more complete picture of customer behavior.

---

# 🛠️ Technology Stack

| Technology              | Purpose                             |
| ----------------------- | ----------------------------------- |
| **Python**              | Data analysis and machine learning  |
| **Pandas**              | Data manipulation and preprocessing |
| **NumPy**               | Numerical computation               |
| **Matplotlib**          | Data visualization                  |
| **Seaborn**             | Statistical visualization           |
| **Scikit-learn**        | Machine learning                    |
| **Logistic Regression** | Churn classification                |
| **Jupyter Notebook**    | Interactive analysis                |
| **Git / GitHub**        | Version control                     |

---

# 📁 Project Structure

```text
Bank-Churners-EDA/
│
├── BankChurners.csv
│   └── Banking customer dataset
│
├── _taux_desabonement_EDA.ipynb
│   └── Exploratory Data Analysis
│       ├── Data exploration
│       ├── Churn analysis
│       ├── Visualizations
│       └── Statistical analysis
│
├── Bank_Logistic_Regression.ipynb
│   └── Logistic Regression
│       ├── Feature preparation
│       ├── Classification
│       └── Model analysis
│
└── README.md
```

The repository currently contains the dataset and two analytical notebooks: an EDA notebook and a dedicated Logistic Regression notebook.

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/SALAH-EO/Bank-Churners-EDA.git
cd Bank-Churners-EDA
```

## 2. Create a Virtual Environment

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

## 3. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## 4. Launch Jupyter

```bash
jupyter notebook
```

Then open either:

```text
_taux_desabonement_EDA.ipynb
```

or:

```text
Bank_Logistic_Regression.ipynb
```

---

# 📌 Project Outcomes

This project demonstrates a complete transition from **raw banking data to actionable analytical insights and predictive modeling**:

```text
                 Raw Customer Data
                         │
                         ▼
                Data Understanding
                         │
                         ▼
                    EDA & EDA
                         │
              ┌──────────┴──────────┐
              │                     │
              ▼                     ▼
       Customer Insights      Statistical Tests
              │                     │
              └──────────┬──────────┘
                         ▼
                  Feature Analysis
                         │
                         ▼
                Logistic Regression
                         │
                         ▼
                 Churn Prediction
                         │
                         ▼
              Retention Opportunities
```

The project demonstrates the ability to combine **data exploration, statistical reasoning, visualization, and machine learning** within a concrete business problem.

---

# 🔮 Future Improvements

The current project provides a strong foundation for a more complete banking churn intelligence system.

Potential extensions include:

### 🤖 Model Comparison

Compare Logistic Regression with:

* Random Forest
* XGBoost
* Gradient Boosting
* Support Vector Machines
* K-Nearest Neighbors

### ⚖️ Class Imbalance Analysis

The churn target is naturally imbalanced, making metrics such as **Precision, Recall, F1-score, ROC-AUC, and PR-AUC** particularly relevant.

### 🧠 Explainable AI

Integrate:

* SHAP
* Feature importance
* Partial dependence analysis

to explain individual churn predictions.

### 🎯 Customer Risk Scoring

Transform binary predictions into actionable customer-risk scores:

```text
0 ─────────────── 1
│                 │
Low Risk       High Risk
```

### 📊 Interactive Dashboard

Build a dashboard using tools such as:

* Power BI
* Tableau
* Streamlit
* Plotly Dash

### 🚀 Deployment

The Logistic Regression model could eventually be exposed through:

```text
REST API
   │
   ▼
Churn Prediction Service
   │
   ▼
Banking Dashboard / CRM
```

This would transform the project from an analytical notebook into an end-to-end **customer churn intelligence solution**.

---

# 🎓 Skills Demonstrated

This project showcases practical experience with:

* **Exploratory Data Analysis**
* **Data Cleaning**
* **Data Visualization**
* **Statistical Analysis**
* **Hypothesis Testing**
* **Customer Segmentation**
* **Feature Analysis**
* **Binary Classification**
* **Logistic Regression**
* **Business-oriented Data Science**
* **Python Data Stack**
* **Jupyter Notebook**
* **Machine Learning Fundamentals**

---

# 🧠 Key Takeaway

> **The goal is not simply to predict churn — it is to understand customer behavior well enough to support better retention decisions.**

By combining **EDA, statistical analysis, customer behavior analysis, and Logistic Regression**, this project demonstrates how raw banking data can be transformed into insights that are relevant to both **data scientists and business decision-makers**.

---

# 👨‍💻 Author

**Salah Eddine Ouirra**

**Data Science & Big Data | AI Engineering | Machine Learning | Data Analytics**

🌐 **Portfolio:** https://salah-eo.vercel.app

---

## 📌 Project Status

**Status:** Completed academic Data Science / Machine Learning project

**Focus:** Banking Customer Churn • EDA • Statistical Analysis • Logistic Regression
