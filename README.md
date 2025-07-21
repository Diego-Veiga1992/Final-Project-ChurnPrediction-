📊 Customer Churn Prediction
This project aims to analyze, visualize, and model customer cancellation behavior (churn), focusing on identifying patterns and predicting which customers are most likely to leave the company.

🧠 Technologies & Tools
Python (Jupyter Notebook)

Libraries:

pandas, numpy – data manipulation and analysis

matplotlib, seaborn – data visualization

scikit-learn, imbalanced-learn – modeling and evaluation

CatBoost, LightGBM – advanced machine learning algorithms

🔍 Project Stages
1. Exploratory Data Analysis (EDA)
Missing value handling

Data type corrections

Distribution analysis

2. Feature Engineering
Created binary column for churn flag

One-Hot Encoding for categorical features

Extracted year, month, and day from subscription start date

Applied resampling to balance target classes

3. Data Visualization
Time-based plots revealed churn consistency across months

Key insights:

Many customers cancel within 2 months (early retention issue)

Average churn time is around 1.5 years

Monthly plans have higher churn concentration

4. Predictive Modeling
Evaluation of several models:

Model	Accuracy	F1 Score	ROC AUC	Score (/10)
LightGBM	0.82	0.73	0.91	⭐ 10.0
CatBoost	0.80	0.73	0.90	⭐ 10.0
Gradient Boosting	0.78	0.69	0.89	⭐ 9.2
Random Forest	0.78	0.68	0.87	⭐ 8.3
Logistic Regression	0.74	0.42	0.58	❌ 0.0
Decision Tree	0.75	0.65	0.85	⭐ 7.5

Top performing models: LightGBM and CatBoost

✅ Conclusion
The complete pipeline provides a strong and accurate foundation for churn prediction.

The company can now:

Anticipate cancellations and act proactively

Focus on early retention (especially within the first 2 months)

Reevaluate monthly plans, which show the highest churn rates
