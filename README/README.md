# Logistical Regression Analysis on the Impact of Quality of Support Network and Educational Attainment on Global Life Satisfaction Scores.

## Research Question
How does the quality of support network and level of educational attainment influence life satisfaction scores, and how can a predictive model, using these key features guide families and communities?

## Executive Summary
This project uses linear and logistic regression to analyse how support networks and education impact life satisfaction, based on global data. The model shows significant influence from 'Quality of Support Network' and 'Educational Attainment.' It achieves an accuracy of 92% and an AUC of 0.90, with perfect recall for Class 1, and 80% with Class 0. Limitations include a low quantity of data points due to country-level aggregation, suggesting further localised studies could provide deeper insights. This evidence-backed research can guide global and local policies to bolster life satisfaction through enhanced educational and community support.

## Project Background
This research aims to explore the correlation between educational attainment, life satisfaction, and the quality of support networks, focusing on how these factors contribute to individual well-being and success. By analysing these specific variables, the study seeks to provide actionable insights for fostering environments that support personal and academic growth. This could also help identify high-risk individuals and communities for targeted interventions.

## Methods
Logistical regression was chosen for it ability to affirn binary classifications. EDA explores data structures and potential biases using tools like correlation matrices, scatter plots, and histograms to assess data distribution and relationships. Ethical considerations include responsibly handling detected biases to ensure model integrity. Severe multicollinearity was identified, risking model overfitting. To address this, variables were integrated into a Socio-Economic Status (SES) metric. Principal Component Analysis (PCA) was utilised to mitigate multicollinearity by transforming correlated variables into uncorrelated components, thus enhancing model stability and reliability. This approach upholds ethical standards by ensuring data accuracy and fairness in modeling outcomes.

## Data Analysis

Hypothesis 

H0 : Null Hypothesis: The quality of an individual’s support network and educational attainment does not influence life satisfaction.

H1 : Alternative Hypothesis: A stronger quality of support network and higher educational attainment is positively associated with higher life satisfaction.

Methodology

EDA (Exploratory Data Analysis)

EDA is an important step to  understand important structures of the data. It can help in detecting any bias which leans toward ethical considerations of responsibly building a model. 

Mean interpolation was utilised to replace a NULL value

Visualisations such as Correlation Matrix, Scatter Plots and Histograms were chosen to find the main characteristics of the distribution of data. There are crucial steps such as Multicollinearity checks which statistically calculate the relationships between variables which may skew building a logistic regression model. 

PCA (Principal Component Analysis) was determined to be the most appropriate to mitigate multicollinearity.  

A correlation matrix is an efficient visual statistical representation of the correlation between two variables. The range is between 1 and -1. 1 being a perfect correlation, 0 is no correlation and -1 is a negative influenced correlation. E.g. if one variable increases the other will decrease.

Scatter plots reveal a positive but not strongly linear relationship between Quality of Support Network and Educational Attainment, with noticeable clustering among countries with high scores in both metrics. Histograms indicate a positive skewness across Educational Attainment and Quality of Support Network, whereas Life Satisfaction scores are more varied, predominantly leaning towards higher values.

The multicollinearity check revealed severe multicollinearity, increasing the risk of overfitting and affecting the model’s sensitivity to changes. To address this, the study will combine the predictors into a Socio-Economic Status (SES) measure, incorporating both quality of support network and educational attainment to create a more streamlined and effective model.

PCA (Principal Component Analysis) combines multiple correlated variables into uncorrelated principal components. PCA mitigates multicollinearity, which can stabilise regression coefficients and improve model reliability.

## Results

![image](https://github.com/user-attachments/assets/f79ba67f-40de-462b-9fbe-29866b4f73ce)

![image](https://github.com/user-attachments/assets/99b81555-5246-49d1-bce1-5d2354cce1be)

![image](https://github.com/user-attachments/assets/b9d5b3cd-8cb0-4eab-8812-245887dbedfd)


## Recommendations
We can confidently reject the null hypothesis in favour of H1.

H1: Higher support network quality and educational attainment positively impact life satisfaction.

This study has statistically verified the positive links between these variables. The unexpected negative coefficients observed may stem from multicollinearity, which contrasts with domain expectations and prior analyses suggesting positive impacts in pair-plots. 
Further iterative analysis is needed to refine feature engineering and improve model interpretation. Enhanced coefficient clarity will help stakeholders better comprehend the model's complexities. The model's robustness is affirmed by strong ROC curve and confusion matrix results, underscoring its accuracy in predicting life satisfaction.

https://www.kaggle.com/datasets/darrylljk/better-life-index-2024-life-satisfaction 

https://skydancer-bytes.github.io/SarahBytes.Github.io/
