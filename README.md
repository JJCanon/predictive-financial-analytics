This project applies statistical analysis and machine learning techniques to financial data using the Bank Marketing Dataset. It includes:
* Descriptive and diagnostic analysis to explore data distributions, trends, and outliers.
* Hypothesis testing to validate insights about customer behavior.
* Predictive modeling (classification and regression) to estimate customer subscription likelihood and financial indicators.
The project is fully documented in Jupyter Notebooks and highlights practical skills in Python, Pandas, Scikit-learn, and data visualization.

# Bank Marketing Campaign Analysis

## Project Overview
This project analyzes a bank marketing campaign dataset to gain insights into client behavior and build predictive models for subscription likelihood.

## Dataset
The dataset contains information from a Portuguese banking institution's marketing campaigns conducted between 2008 and 2013.

**Source:** [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

**Features include:**
- Client demographics (age, job, marital status, education)
- Economic indicators (balance, housing loan, personal loan)
- Campaign details (contact type, day, month, duration)
- Previous campaign outcomes

**Target variable:** `deposit` - whether the client subscribed to a term deposit (yes/no)

## Project Structure
bank-marketing-analysis/
├── financial-analysis.ipynb # Main analysis notebook
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── data/ # Dataset directory (not included in repo)
└──── bank.csv # Dataset file

## Key Steps Performed

1. **Descriptive Analysis**: Exploratory data analysis with visualizations and statistical summaries
2. **Hypothesis Testing**: 
   - T-test for call duration by housing loan status
   - ANOVA for balance across job types
   - Chi-square test for personal loan by marital status
3. **Predictive Modeling**:
   - Classification: Predicting term deposit subscription (Logistic Regression, Decision Tree)
   - Regression: Predicting account balance (Linear Regression)

## Results Summary

### Classification Results:
- **Logistic Regression**: 82.5% accuracy, F1-score: 0.812
- **Decision Tree**: 79.4% accuracy, F1-score: 0.780 (improved with pruning)

### Regression Results:
- **Linear Regression**: R² = 0.0385 (account balance difficult to predict with available features)

## Installation & Usage

1. Clone the repository:
```bash
git clone https://github.com/your-username/bank-marketing-analysis.git
cd bank-marketing-analysis
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the jupyter notebook
```bash
jupyter notebook financial-analysis.ipynb
```
## Dependencies
* Python 3.7+
* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* scipy
* jupyter
## Author
Juan José Gabriel Cañón Díaz
