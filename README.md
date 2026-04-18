Project Title
Understanding Factors Affecting Bike Usage

Introduction / Overview
Yulu is India's leading micro-mobility service provider, which offers unique vehicles for daily commute. With the mission to eliminate traffic congestion in India, Yulu provides the safest commute solution through a user-friendly mobile app to enable shared, solo, and sustainable commuting.
Recentlly, they suffered dips in its revenue, and they want to understand the factors affecting the demand for these bikes in the Indian market.

Dataset:
- The data was obtained from kaggle.
- The dataset contains datetime, season, holiday, workingday, weather, temp, atemp, humidity, windspeed, casual, registered, and count (which has been renamed as 'total_users' in this project).

Objective:
Find out which variables are significant in predicting the demand for shared bikes in the Indian market.

Methods:
- The methods used are data inspection and standardization, visualizations.
- Further analysis used two sample t-tests, and due to groups' variances significantly differ from each other, Welch's ANOVA and Games-Howell post-hoc test were used.
- Multiple linear regression were used with robust standard errors (HC3) to a logged model to ensure inference is valid.
- Breush-Pagan and White tests are used to check for evidence of heteroscedasticity.

Key Findings:
- Bike demands or rentals were positively affected by hour of the day (peaks in the afternoon around 3pm, lowest in the early morning around 3am).
- June-August has highest bike rentals compared to baseline January.
- Saturday has highest bike rentals compared to baseline Monday.
- Temperature has positive effect on bike rentals.
- Misty weather has negative effect on bike rentals.
- Light precipitation weather and windspeed have weak negative effects on bike rentals.
- Heteroscedasticity and non-normal residuals were found in the dataset. After log transformation, residuals are normalized but heteroscedasticity persists.

How to Run:
- Open the notebook file (Yulu Bikes.ipynb) in Jupyter Notebook or JupyterLab.
