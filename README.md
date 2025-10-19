## Click to Cart: A Predictive Modelling Task
This project aims to predict whether a user will make a purchase based on their session-level data. The dataset contains features such as time spent on the site and pages viewed, which are highly correlated with purchase behavior. 



This task is approached as a supervised learning problem, utilizing Random Forest and XGBoost classifiers to build the predictive model. 

## Project Workflow
The project is broken down into four main stages:


Exploratory Data Analysis (EDA): The initial analysis involved visualizing numerical and categorical features using histograms and bar plots, respectively. A correlation matrix and boxplots were used to understand feature relationships and detect outliers. A key finding was the skewness in the Cart_value feature, which was addressed by applying a log transformation to normalize its distribution. Additionally, the Browser_Refresh_Rate feature was dropped due to its low correlation with the target variable. 





Data Preprocessing: Categorical features were encoded using a One-Hot Encoder, and all features were scaled using a StandardScaler to prepare the data for modeling. 

Model Selection & Training:


Random Forest Classifier: An ensemble model of decision trees that reduces variance and captures non-linear effects by training on different subsets of the data and aggregating the results. It uses Gini impurity to find the best splits when building trees. 




XGBoost Classifier: A boosting-based ensemble model that trains models sequentially, with each new model correcting the errors of its predecessor. It focuses on reducing bias and uses residuals to guide the learning process. 






Comparative Analysis: Both models performed well, but the Random Forest Classifier achieved a slightly higher accuracy. This is likely because Random Forest is more robust to noise and the features in this dataset are largely independent, which limits the advantage of XGBoost's iterative error-correction approach.
