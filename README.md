# Bike Sharing Demand Prediction

## You will find everything you need in the /Project folder

---

This project aims to predict the bike sharing demand using the Bike Sharing Demand dataset obtained from Kaggle. The prediction is performed using AutoGluon, a powerful library for automated machine learning. In this project, we will cover the following steps:

1. Data Download and Preparation
2. Feature Creation and Data Analysis
3. Model Training With AutoGluon
4. Model Performance Comparison
5. Competition Report


## 1. Data Download and Preparation
To get started, please follow the steps below:


1. Download the Bike Sharing Demand data from Kaggle.
2. Install the Kaggle CLI and configure it with your Kaggle API token.
3. Use the Kaggle CLI to download and unzip the Bike Sharing Demand dataset into your preferred environment (e.g., Sagemaker Studio or local development).
4. Load all datasets from the Bike Sharing Demand competition into Pandas using the read_csv() function.
5. View the dataframe in your Jupyter notebook to ensure the data is loaded correctly.


## 2. Feature Creation and Data Analysis
In this step, we will create a new feature by extracting data from an existing feature column. Additionally, we will create a histogram of all features in the train dataset to gain insights into the data.

1. Choose one feature column and extract data from it to use in a new feature column.
2. Add the new feature to both the train and test datasets.
3. Create a matplotlib image showing histograms of each feature column in the train dataframe.


## 3. Model Training With AutoGluon
Next, we will train a Tabular Prediction model on the training set using AutoGluon. AutoGluon provides an automated way to train and tune models, making it easier to achieve good performance.

1. Use the TabularPredictor class from AutoGluon to create a predictor by calling .fit().
2. Optionally, change the hyperparameters when training the Tabular Prediction model by providing additional arguments in the .fit() function.


## 4. Model Performance Comparison
In this step, we will compare the performance of different models trained using AutoGluon and select the best one. We will also make predictions with the trained model on the test dataset.

1. Submit a prediction submission from the trained AutoGluon Tabular Predictor to Kaggle for scoring.
2. Graph the changes of the model evaluation metric after each model iteration using matplotlib or a similar tool.
3. Graph the changes to the Kaggle competition score after each model iteration using matplotlib or a similar tool.


## 5. Competition Report
Finally, we will compile a competition report summarizing the results of the training run and the impact of exploratory data analysis (EDA) on model performance.

1. Identify the best model from AutoGluon based on the results obtained from ``fit_summary()`` or ``leaderboard()``.
2. Discuss how EDA led to discoveries in the data that impacted model performance.
3. Explain why changes to hyperparameters affected the outcome of the model's performance. Provide a table outlining the hyperparameters used along with the corresponding Kaggle scores.
4. Include suggestions to make the project stand out, such as adding additional features, performing multiple rounds of hyperparameter tuning, testing different algorithm types, and creating more visualizations.


### Suggestions to Make Your Project Stand Out:

* Add more than one feature to the dataset and train models to see if it improves the Kaggle score.
* Perform multiple rounds of hyperparameter tuning to see if it improves the Kaggle score.
* Test individual algorithm types (KNN, Neural Nets, RF, XGBoost, etc.) and write a detailed analysis of which one performs better on this dataset.
* Create more visualizations for the report