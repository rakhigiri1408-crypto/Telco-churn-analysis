# Telco-churn-analysis
Exploratory data analysis and churn prediction model for a telecom company using SQL, Python and Logistic Regression. Identifies high-risk customer segments causing $52K/month revenue loss.
# Telecom Customer Churn Analysis

## Business Problem
A telecom company is losing 26.5% of its customers every quarter. 
This project identifies which customers are most likely to churn 
and recommends actions for the retention team.

---

## Key Business Insights

| Insight | Finding |
|---------|---------|
| Overall Churn Rate | 26.5% , 1 in 4 customers leaving |
| Highest Risk Contract | Month-to-month customers churn 3x more than long-term |
| Payment Red Flag | Electronic check users churn 4x more than auto-pay users |
| High Risk Segment | New customers (<12 months) paying >$65/month |
| Revenue Impact | 637 high-risk customers = ~$52,000/month revenue loss |

---

## Business Recommendations

1. **Target month-to-month customers** with upgrade offers to annual contracts
2. **Incentivise auto-pay setup** - electronic check users are low engagement and high churn risk
3. **Prioritise retention budget** on customers with tenure under 12 months and monthly charges above $65
4. **Senior citizen segment** needs separate retention strategy - second highest churn driver

---

## Tools Used
- Python (Pandas, Scikit-learn, Matplotlib, Seaborn)
- SQL (SQLite)
- Google Colab

## Dataset
IBM Telco Customer Churn — [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
7,043 customers | 21 features

## Model Performance
- Algorithm: Logistic Regression
- Accuracy: 79%
- Key limitation: 192 false positives - retention budget may be wasted on customers who were not going to churn
