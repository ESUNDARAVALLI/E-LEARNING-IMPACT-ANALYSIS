E-learning Impact Score Prediction:
This project develops a stacked regression model to predict the E-learning Impact Score of learners using survey-based data. The methodology integrates multiple machine learning algorithms with hyperparameter tuning and a meta-model to improve predictive performance.

Dataset:
File: E-learning_Impact_Score1.csv
Target Variable: E-learning_Impact_Score

Features Used:
Age
Level_of_Education
Types_of_content
Hours_spent_weekly
Purpose_of_content
Learning_preferences
E-learning_platforms

Methodology:
Data Preprocessing
Label encoding of categorical variables.
Separation of features (X) and target variable (y).
Base Models with Hyperparameter Tuning:
  RandomForestRegressor
  XGBRegressor
  LGBMRegressor
  CatBoostRegressor
  MLPRegressor
Stacking Framework
Five-fold cross-validation.
Out-of-fold predictions generated for meta-model training.
Meta-Model:
  ElasticNet regression.
  Hyperparameter tuning performed using GridSearchCV.
Model Evaluation Metrics:
  Root Mean Squared Error (RMSE)
  Mean Absolute Error (MAE)
  R² Score

Results:
Metric	Value
RMSE	  0.8831
MAE	  0.6840
R²	  0.8663

The results indicate that the model explains approximately 87 percent of the variance in E-learning Impact Scores, with an average prediction error of less than one unit.

Visualization:
A scatter plot of actual versus predicted scores illustrates the closeness of the model’s predictions to the true values
