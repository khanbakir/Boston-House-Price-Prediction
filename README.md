🏡 Boston House Price Prediction
This project analyzes the Boston housing dataset and builds several machine learning models to predict house prices. It serves as a practical demonstration of a complete data science workflow, from exploratory data analysis (EDA) to predictive modeling and evaluation.

📋 Project Structure
The core of this project is the Boston_House_Price_Prediction.ipynb Jupyter Notebook, which contains the complete analysis and code.

The project workflow includes:

Data Loading & Initial Analysis: Loading the dataset and examining its structure and summary statistics.

Data Preprocessing: Preparing the data for machine learning models.

Model Building: Implementing and training different regression models.

Model Evaluation: Assessing model performance using key metrics.

🔍 Analysis and Key Findings
Exploratory Data Analysis (EDA)
The dataset contains 506 entries and 15 columns, including the target variable medv (median house value).

I used a correlation heatmap to visualize the relationships between all features. The heatmap revealed strong correlations between several features, which is crucial for understanding the dataset before building predictive models.

Data Preprocessing
I split the dataset into training (70%) and testing (30%) sets to ensure the models are evaluated on unseen data, which helps to avoid overfitting.

I applied MinMaxScaler to normalize the features. This step ensures that all features contribute equally to the model training process, preventing features with larger values from dominating the learning algorithm.

Predictive Models
I implemented and evaluated three regression models:

Multiple Linear Regression: This model tries to find a linear relationship between the input features and the house price.

Polynomial Regression: An extension of linear regression that models the relationship as a polynomial, which can capture more complex, non-linear patterns.

K-Nearest Neighbors (KNN): A non-parametric, lazy learning algorithm that predicts the house price based on the average price of its nearest neighbors in the feature space.

📊 Model Performance
Model	R²-score	MAE	MSE	RMSE
Multiple Linear Regression	0.75	2.95	17.84	4.22
Polynomial Regression (with nox & dis)	0.70	0.86	1.30	1.14

Export to Sheets
The Multiple Linear Regression model achieved an R²-score of 0.75, indicating that it can account for approximately 75% of the variance in the house prices. This suggests that the model is a strong fit for the dataset.
