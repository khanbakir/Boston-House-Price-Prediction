#Boston House Price Prediction
This project analyzes the Boston housing dataset and builds several machine learning models to predict house prices. It serves as a practical demonstration of a complete data science workflow, from exploratory data analysis (EDA) to predictive modeling and evaluation.

#Project Structure
The core of this project is the Boston_House_Price_Prediction.ipynb Jupyter Notebook, which contains the complete analysis and code.

#The project workflow includes:

1. Data Loading & Initial Analysis: Loading the dataset and examining its structure and summary statistics.

2. Data Preprocessing: Preparing the data for machine learning models.

3. Model Building: Implementing and training different regression models.

4. Model Evaluation: Assessing model performance using key metrics.

#Analysis and Key Findings
1. Exploratory Data Analysis (EDA): The dataset contains 506 entries and 15 columns, including the target variable medv (median house value). I used a correlation heatmap to visualize the relationships between all features. The heatmap revealed strong correlations between several features, which is crucial for understanding the dataset before building predictive models.

2. Data Preprocessing: I split the dataset into training (70%) and testing (30%) sets to ensure the models are evaluated on unseen data, which helps to avoid overfitting.

3. I applied MinMaxScaler to normalize the features. This step ensures that all features contribute equally to the model training process, preventing features with larger values from dominating the learning algorithm.

4. Predictive Models: I implemented and evaluated three regression models:

(i). Multiple Linear Regression: This model tries to find a linear relationship between the input features and the house price.

(ii). Polynomial Regression: An extension of linear regression that models the relationship as a polynomial, which can capture more complex, non-linear patterns.

(iii). K-Nearest Neighbors (KNN): A non-parametric, lazy learning algorithm that predicts the house price based on the average price of its nearest neighbors in the feature space.

