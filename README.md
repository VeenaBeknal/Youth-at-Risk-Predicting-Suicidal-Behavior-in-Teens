# Youth-at-Risk-Predicting-Suicidal-Behavior-in-Teens

## Overview

The percentage of high school students reporting suicidal thoughts rose from 16% to 22% (CDC) from 2011 to 2021. Suicide is the second leading cause of death for individuals aged 10–24,they increased by 52.2% from 2000–2021. The YRBS survey dataset is ideal for risky behavior analysis like suicide risk due to its comprehensive, nationwide data on youth behaviors and mental health. Our goal is to predict suicidal behavior in high-school students Machine Learning techniques. The target variable for the project is the question “During the past 12 months, did you ever seriously consider attempting suicide?”. The rise in mental health issues underscores the need for predictive models to identify at-risk youth and intervene early.

## Data Overview

The main objective of the project is to predict the risk factor of a teen committing suicide by following data mining and machine learning techniques to discover hidden patterns. Raw dataset was converted into a form suitable for analysis using feature mapping techniques using the Appendix C provided by YRBSS. This the dataset which is available in YRBS Survey dataset for the year 2021. This was dataset was selected to perform data analysis of youth suicide behavior which has 17,232 rows (survey respondents) and 109 columns (questions). This is a survey dataset for the year 2021 which contains 17,232 rows (survey respondents) and 109 columns (questions). Responses marked as "Missing" indicate question skipped by respondents and majority of data is categorical. 

## Data Preprocessing

Data preprocessing was performed on the dataset such as checking for missing and null values since this is a survey data we cannot say the data is missing. I have choosen to mark them as skipped or missing depends on the variable. Dropped columns where 40% ofvalues were missing, also we have dropped irrelevant features like site, height_ft, weight_in, etc. Used KNN based imputationon height and weight feature, later applied min-max scaling for continuous features. Performed one-hot encoding on categorical featuressince most of our data is categorical and finally we have 301 columns.

## Data Statistics

Conducted a t-test to examine whether there is a difference in height between teens who have considered committing suicide in the past 12 months. The results indicate a statistically significant difference in height of teens. Similarly, t-test was performed on weight and BMI category features. The results indicate thatthere is statistically significant difference with these features. For Categorical Variable we used Chi-square test for categorical variables to check goodness of fit. To assess whether there is any kind of relationship exists between our target and the independent variables.Using Cramer’s V, which determines the strength of the relationship between categorical features and target variable.

## EDA

In exploratory data analysis univariate and bivariate analysis was done. Explore the file for detail analysis on the outcomes of each analysis.

## Feature Engineering

This project calculated “Suicide Risk Score” can help identify the risk profiles of respondents more prone to suicide, this is based on bucketing the predicted probabilities which is data-driven tool to identify very high risk respondent. Height and weight alone were insufficient for analyzing suicide risk, so we calculated BMI and grouped it into categories for better analysis. Created a tobacco products to use feature by combining the nicotine products, and we found that teens who use any kind tobacco products are two times likely to commit suicide.

## Machine Learning 

Machine learning models were selected mainly classification as this was the binary classification problem. Logistic regression, Random Forest, XGboost and Naive Bayes models were selected. Based on performance XGBoost achieved the highest accuracy (84.52%). Based on recall Strength with the highest recall (53.43%), XGBoost minimized misclassification of youth at-risk, excelling at identifying true positive cases.

## Conclusion

- Females are twice as likely as men to consider suicide.
- Feeling sad and hopeless has a strong positive correlation with increased suicide risk.
- Sexual minorities experience significantly elevated suicide risk rates compared to heterosexual individuals, with bisexual individuals facing the most severe disparity.
- This study can be used by teachers, counselors, and other concerned authorities to take proactive measures to intervene for very high-risk and high-risk students.
- Preventive measures can help in identifying struggling youth and provide them with the necessary support.

## File Structure

`YRBS data mining - Data Mapping and Data Processing.ipynb`: This python file contains the data mapping from raw file and data preprocessing

`YRBS_data_mining_EDA_Modeling.ipynb`: This file contains the EDA and predictive modeling of the project

## Contact Information

For inquiries or feedback, contact:

- Veenaramesh Beknal: veenaramesh.beknal@sjsu.edu

Explore the project and leverage insights from the Youth at Risk: Predicting Suicidal Behavior in Teens!

"Awareness is like the sun. When it shines on things they are transformed" -- Thick Nhat Hanh
