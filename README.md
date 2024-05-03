# ES-thesis-24
My Environmental Science Honors thesis for UC Berkeley, Class of 2024. Predicting plastic policy effectiveness in Indonesia.

- **Title** - Harnessing Machine Learning Insights for Effective Policy Projections: A Study of Single-Use Plastic Bag Bans in Indonesia
- **Keywords** - Indonesia, policy, single-use plastic bag ban, predictive modeling, causal inference
- **Author** - Sandya Wijaya, Advised by Kate O'Neill

## Paper Abstract
Plastic pollution poses a significant environmental challenge globally, prompting governments to implement policies aimed at mitigating its adverse effects. In this study, I employ predictive modeling techniques to predict the effectiveness of plastic policies in cities of Indonesia where such interventions have not been previously employed.  Specifically, I explored single-use plastic bag bans. I explored 9 different models but the best performing one was a XGBoost model with default parameters. I also performed causal inference analysis, using outcome regression and inverse propensity weighting to confirm that there is a causal link between plastic bag bans and plastic pollution. My findings reveal population as a key determinant influencing the impacts of plastic bag bans on pollution levels, that there is a 2 year delay between when a ban is implemented to when reported numbers start to change, and that coastal cities are more likely to see decreases in plastic if a ban is implemented. By elucidating the impacts of plastic bag bans effectiveness, this study informs strategic resource allocation and policy formulation efforts, contributing to the advancement of environmental governance practices in Indonesia and beyond.

## Files
- **Data** : Comprises of 3 main types of data 1) plastic (AMOUNT OF TRASH, TRASH COMPOSITION) 2) indicators (GDP, Gini Index, HDI Index, Land Area, Population) which are both secondary datasets collected online 3) ban (bans_over_time) which I made.
- **merging.ipynb** : To merge all datasets together before working with it.
- **EDA + Feature Engineering.ipynb** : Doing initial exploration and feature engineering.
- **Confounder.ipynb** : Causal analysis using unconfoundedness techniques such as outcome regression, matching, inverse propensity weighting. References: Data 102 Spring 2024 Lab 8.
- **Modeling.ipynb** : Predictive modeling using linear regression, LSTM, SVM, LSTM (find code in lstm_googlecolab folder, which is done on the cloud due to lack of power locally), Gamma GLMs, XGBoost, KNN, Decision Trees, Random Forest. Hyperparameter tuning using RandomizedSearch and GridSearch.
- *All other files and CSVs are a result of saving merged and edited CSVs from the above code notebooks.*
