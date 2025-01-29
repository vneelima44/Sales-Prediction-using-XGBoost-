The Approach
In this project, I built a sales prediction model using XGBoost to predict the sales of retail outlets based on various features like store type, outlet size, and product categories. Here’s how I approached it:
Data Collection: Used a dataset available on Kaggle-https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets/data
Data Preprocessing: Handled missing values/duplicate values , and transformed categorical features into numerical ones.
How? 
I applied both univariate and multivariate imputation techniques for handling missing values. These included:
Mean and Median Imputation
Random Forest Imputation
Interpolation (finally chosen)
Why Interpolation?: The data distribution was continuous and fairly spread across, making interpolation the best method. I compared results visually through distribution plots and found that interpolation provided the most accurate fill for missing data, preserving the overall distribution and preventing skewed predictions.(Visualization attached for refernce)
Feature Engineering: Created new features from the existing ones to better capture patterns in the data.
Exploratory Data Analysis (EDA): a. Visualized &  Analyzed the distribution of sales and identified potential outliers.
Modeling:
Tried two advanced machine learning algorithms—Random Forest and XGBoost—to predict sales and evaluate model performance using Root Mean Squared Error (RMSE). Both models provided valuable insights, but XGBoost outperformed in terms of accuracy, helping us get closer to the true sales numbers.
Evaluation: Used cross-validation to validate model performance, achieving an R² score of 0.59 on the test set.

