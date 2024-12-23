Economic Effects of Healthcare for Vietnamese Citizens
===
Final Group Report - MATH4322

University of Houston

Course: MATH4322  

Team Members
Riches Dang,
Chris Do,
Justin George,
John Pham

Project Overview
---
Healthcare is essential to human societies, yet the costs associated with medical care vary widely across the globe. This project analyzes the economic effects of healthcare expenditure on Vietnamese citizens using data from the Vietnam World Bank Living Standards Survey. The dataset contains 27,765 observations and 12 variables concerning medical expenses at the individual level.

Research Question
---
What is the economic analysis of healthcare expenditure for medical visits in the context of the Vietnamese healthcare system, accounting for variations in cost factors such as geographic location, patient demographics, and specific service components?

Methodology
---
**Linear Regression Model**

Team Members: Chris Do, John Pham

A Linear Regression model was implemented to predict medical expenses based on various predictors. The final regression model used predictors such as age, education, and insurance, while excluding insignificant predictors like gender and injury. The model's key equation is:

Evaluation Metrics:

Mean Squared Error (MSE): Averaged 33% across 10 iterations.
Model Selection Criteria: AIC, BIC, and Adjusted R-Squared values were used to compare models, with the second model selected as the best fit.

**Bagging Method**

Team Member: Justin George

Bagging was employed to reduce variance and improve the robustness of predictions. By aggregating results from 500 decision trees, the 

MSE was minimized to 0.1030. A Variable Importance Measure plot was generated to assess the influence of predictors.

Results
---
**Linear Regression Results**

R-Squared: 0.1293 (indicating the model explains 12.93% of variance in the response variable).

F-Statistic: The p-value (< 2.2 × 10^-16) suggests that at least one predictor significantly affects healthcare expenditure.

**Bagging Results**

MSE: 0.1030, translating to an average prediction error of $1007 in healthcare expenses per family after accounting for logarithmic scaling.

Key Variables: Education and commune were identified as critical factors impacting healthcare costs.

Dataset
---
Source: Vietnam World Bank Living Standards Survey

Access Method: R package Ecdat, item VietNamI

Response Variable: lnhhexp (logarithm of total medical expenditure)

Predictors: Age, education, marital status, insurance, geographic commune, and more.


Conclusion

The project provides insights into the economic implications of healthcare expenditures in Vietnam, highlighting significant factors like education and geographic location. The study emphasizes the need for targeted policies to address disparities in healthcare access and costs.


