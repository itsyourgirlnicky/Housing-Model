# REAL ESTATE SALES PREDICTION MODEL

## Project Overview

In the fast-paced world of real estate, providing clients with accurate insights is key. Real estate agencies guide homeowners through crucial decisions like pricing, market analysis, and property inspections. This project aims to equip agencies with a powerful regression-based tool. This tool predicts potential property value increases based on factors like bedrooms, year built, floors, living space, condition, and location. With this model, agencies can offer tailored advice, ensuring clients make informed decisions for maximizing returns in the competitive market

### Business Problem

In King County,stakeholders in the real estate industry face challenges in understanding the factors influencing property valuation and market trends. This study seeks to address these challenges by analyzing the complexies between property features, location-related factors, market preferences, and temporal dynamics. By gaining insights into these factors, stakeholders can make more informed decisions regarding property investments, pricing strategies, and market positioning. Ultimately, the goal is to provide actionable insights that empower stakeholders to navigate and succeed in the dynamic King County real estate market
### The Data

King County, Washington, located in the northwestern United States, boasts a vibrant housing market anchored by the bustling city of Seattle. Over the years, the county has seen remarkable growth, driven by its thriving economy and cultural significance. This has attracted a surge of residents, spurring high demand for housing across urban and suburban landscapes. Seattle, renowned for its striking skyline, has become particularly desirable for tech professionals and city enthusiasts alike. Known for its competitiveness, King County's real estate market offers diverse neighborhoods catering to various preferences, from historic districts to contemporary suburban developments.

**Target Variable**

price: Sale price of the house .

**Unique identifier**

id - Unique identifier for a house

**Property Characteristics:**

bedrooms: Number of bedrooms.

bathrooms: Number of bathrooms.

sqft_living: Square footage of living space in the home.

sqft_lot: Square footage of the lot.

floors: Number of floors (levels) in the house.

waterfront: Indicates whether the house is on a waterfront (categorical: YES/NO).

view: Quality of view from the house, categorized into various types.

condition: Overall condition of the house, categorized based on maintenance.

grade: Overall grade of the house, reflecting construction and design quality.

**Additional Features:**

sqft_above: Square footage of house apart from the basement.

sqft_basement: Square footage of the basement.

yr_built: Year when the house was built.

yr_renovated: Year when the house was renovated.

zipcode: ZIP Code of the property.

lat: Latitude coordinate of the property.

long: Longitude coordinate of the property.

sqft_living15: Square footage of interior housing living space for the nearest 15 neighbors.

sqft_lot15: Square footage of the land lots of the nearest 15 neighbors.
### Key Points

# **OBJECTIVES**


**Main Objective:**

The primary objective of this project is to construct a predictive regression model to aid real estate agencies in advising clients on house prices. The model is designed to forecast potential fluctuations in property value based on property characteristics, providing valuable insights to empower clients in making well-informed investment decisions.

**Specific Objectives:**

i). Identify Key Factors Influencing House Prices:

Examine various features, such as bedrooms, bathrooms, and square footage, to determine their impact on sale price. Investigate location-related attributes like zip code and geographic coordinates to further understand their influence on property prices.

ii). Evaluate Model Performance:

Utilize metrics such as mean squared error, R-squared values, and residual analysis to assess the model's effectiveness in accurately predicting house prices.

iii). Offer Actionable Recommendations:

Provide practical suggestions to real estate agencies for enhancing profitability and market presence. Utilize insights derived from the model to optimize marketing strategies and improve overall decision-making process

# **TABLE OF CONTENT**
1.   Data Preparation
2.   Data cleaning
1.   Exploratory data analysis
2.   Statistical Analysis
1.   Modelling
2.   Regression Results
1.   Conclusion
2.   Recomendations

# **REGRESSION RESULTS**

Polynomial Regression is the preferred model beacuse from the evaluation it has the highest R-squared value of 0.71

The features below impact price such that an increase will cause an increase in the price of the property.
'bedrooms','bathrooms', 'sqft_living','floors', 'waterfront','view''condition', 'grade', 'sqft_above','sqft_basement', 'yr_renovated', 'sqft_living15','renovated', 'basement'. 

On the other hand yr_built has a negative impact on price since the older the house the lower value it has which is shown by its negatice coefficient 

# **CONCLUSIONS**

**Limitations**
1.   The dataset could have more property based characteristics
2.   Multicollinearity:The presence of correlated predictors (e.g., square footage and number of bedrooms) can lead to multicollinearity issues, making it challenging to interpret the individual effects of each feature accurately

1. Assumption Violations:Polynomial regression assumes linearity between predictors and the target variable, which may not hold true in all cases. Violations of this assumption can lead to biased estimates and unreliable predictions.

1. Overfitting: Polynomial regression models, particularly those with high degrees, are susceptible to overfitting, where the model fits the training data too closely and may not generalize well to unseen data.




Overall the model was the best fit model for this predictions

# **RECOMENDATIONS**

1.   Feature Enrichment: Enhance the dataset with additional property-based characteristics like property to amenities and architectural style to provide a more comprehensive understanding of factors influencing house prices.

2.   Multicollinearity Management: Address multicollinearity by employing techniques such as feature selection, principal component analysis (PCA), or regularization methods like ridge regression or Lasso regression to prioritize important predictors and stabilize the model's interpretability.

1.   Assumption Validation: Before using polynomial regression, verify the linearity assumption between predictors and the target variable. If non-linearity is observed, explore alternative regression techniques like generalized additive models (GAMs) or spline regression for better capturing complex relationships.
2. Overfitting Prevention: Prevent overfitting by balancing model complexity and generalizability through techniques such as cross-validation, regularization, or model selection criteria. Consider collecting more data or using bootstrapping to improve robustness and reduce noise in the model.

