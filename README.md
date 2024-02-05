# BankChurnBinaryProbability
The full-process Jupyter notebook with EDA and XGBoost predictive ML model building/evaluation for building a model to predict bank churn.
In this notebook, there are basic EDA practices, feature engineering, model tuning and building, model evaluation, synthetic minority oversampling technique, and some basic dataframe restructuring to deliver a final product in the for that a stakeholder wants. 

First there was data exploration, then removal of potentially unethical categories for prediction. Key categories were changed into snakecase, with the exception of 'Exited', kept the same for final submission purposes. Dummies were made for geography. After this, Tenure was engineered into three categories; new, middle, and old. Were I to perform this data again, I might not engineer that feature. 

Scoring and parameters for tuning were defined, then GridSearchCV was utilized to tune our model. The initial constructed model had lower recall and precision than hoped, so a new model was developed using data that was synthesized using SMOTE. The idea here was to increase recall, precision, and f1. The final model significantly outperformed the initial in testing for these measures and was utilized to predict the probability outcomes for customers churning from the bank in the test dataset.

The notebook ends with some structuring of arrays outputted by our model, then construction of a final dataframe. At the end of this process, our 2-column submission dataframe was completed.
