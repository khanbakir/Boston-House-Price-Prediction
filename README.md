# Boston House Price Prediction

This project is a comprehensive analysis and predictive modeling exercise focusing on forecasting house prices in Boston using various machine learning algorithms. It demonstrates a complete data science workflow, from **exploratory data analysis (EDA)** to **predictive modeling** and **evaluation**.

---

### Project Overview

The project is encapsulated in a single Jupyter Notebook: `Boston_House_Price_Prediction.ipynb`. It follows a structured approach to solving the regression problem:

1.  **Data Loading & Initial Analysis**: Understanding the dataset's structure, features, and basic statistics.
2.  **Data Preprocessing**: Cleaning and preparing the data for model training.
3.  **Model Building**: Implementing and training different regression models.
4.  **Model Evaluation**: Assessing model performance with relevant metrics.

---

### Key Findings and Methodology

#### **Exploratory Data Analysis (EDA)**

* The dataset contains **506 entries** and **15 columns**, including the target variable `medv` (median house value).
* A **correlation heatmap** was generated to visualize the relationships between all features. This step helped to identify which variables have the strongest influence on the `medv` variable, such as `rm` (average number of rooms) and `lstat` (percentage of lower status population).

#### **Data Preprocessing**

* The data was split into **training (70%)** and **testing (30%)** sets to ensure the models are evaluated on unseen data, which prevents overfitting.
* **MinMaxScaler** was used to normalize the features, scaling them to a range between 0 and 1. This is a crucial step for many machine learning algorithms to perform optimally.

#### **Predictive Models**

I implemented and evaluated three different regression models to predict house prices:

1.  **Multiple Linear Regression**: This model established a linear relationship between multiple independent variables and the house price.
2.  **Polynomial Regression**: An extension of linear regression that can capture non-linear relationships within the data, providing a more flexible model.
3.  **K-Nearest Neighbors (KNN)**: A non-parametric model that makes predictions based on the average value of its closest data points.

---

### Model Performance

| Model | R²-score | MAE | MSE | RMSE |
| :--- | :--- | :--- | :--- | :--- |
| **Multiple Linear Regression** | 0.75 | 2.95 | 17.84 | 4.22 |
| **Polynomial Regression** | 0.70 | 0.86 | 1.30 | 1.14 |

The **Multiple Linear Regression model** achieved the highest performance with an **R²-score of 0.75**. This means the model explains approximately 75% of the variability in the house prices, indicating a strong predictive capability.

---

### How to Run the Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/khanbakir/Boston-House-Price-Prediction.git](https://github.com/khanbakir/Boston-House-Price-Prediction.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd Boston-House-Price-Prediction
    ```
3.  **Install the necessary libraries:**
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
4.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook "Boston House Price Prediction.ipynb"
    ```
