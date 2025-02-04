
📊 **Multiple Regression Modeling: Predicting U.S. GDP**
📝 **Project Overview**
This project explores the factors influencing the Gross Domestic Product (GDP) of the United States using multiple regression modeling. The dataset consists of economic indicators from 1970 to 2023, and the goal is to develop an accurate predictive equation for GDP using a stepwise regression approach.

 **Dataset Description**
The dataset contains six explanatory variables related to economic performance:

* Unemployment Rate (%): Measures the percentage of unemployed individuals.
* Government Expenditure (Billion $): Represents government spending.
* Interest Rate (%): The cost of borrowing money.
* Exports (Billion $): The value of goods/services sold to other countries.
* Imports (Billion $): The value of goods/services purchased from other countries.
* Recession Indicator (0/1): A binary variable indicating whether the data was collected post-2009 (after the Great Recession).
  
**Expected Relationships**
Before modeling, we hypothesized the following relationships:

* Unemployment Rate ⬇️ GDP (Inverse relationship)
* Government Expenditure ⬆️ GDP (Direct relationship)
* Imports ⬇️ GDP (Inverse relationship)
* Exports ⬆️ GDP (Direct relationship)
* Interest Rate ⬆️ GDP (Direct relationship)
* Recession ⬆️ GDP (Expected recovery post-recession)
  
** Regression Modeling Approach**
The forward stepwise regression method was used to iteratively build the best-fit model. This method:

Starts with the most correlated predictor (Imports)
Adds variables one by one based on statistical significance
Stops when adding more variables does not significantly improve the model
Final Regression Model
After multiple iterations, the best model includes: 
✔️ Imports – Contrary to expectations, an increase in imports correlates with higher GDP.
✔️ Government Expenditure – Positively impacts GDP.
✔️ Unemployment Rate – Negatively impacts GDP, as expected.

Dropped variables: Exports, Interest Rate, Recession Indicator (not statistically significant).

Final Regression Equation
𝐺
𝐷
𝑃
=
𝛽
0
+
𝛽
1
⋅
Import Amount
+
𝛽
2
⋅
Government Expenditure
+
𝛽
3
⋅
Unemployment Rate
+
𝜖
GDP=β 
0
​
 +β 
1
​
 ⋅Import Amount+β 
2
​
 ⋅Government Expenditure+β 
3
​
 ⋅Unemployment Rate+ϵ

 
**Results & Insights**
* Imports ($1B increase) → GDP rises by $3.67B
* Government Expenditure ($1B increase) → GDP rises by $1.59B
* Unemployment Rate (1% increase) → GDP drops by $230.95B

**Model Assumptions Checked**
* Linearity 
* Constant Variance of Errors 
* Independence of Errors  (Correlation of residuals = 0.526, indicating a medium-strength pattern)
* Normal Distribution of Errors 
