# Rain Prediction using Logistic Regression

## Project Overview

This project aims to predict whether it will rain the next day in Australia by training a Logistic Regression model. The analysis involves a comprehensive workflow including data cleaning, exploratory data analysis (EDA), feature engineering, and model evaluation. The model is built using Python and leverages various data science libraries to process the data and assess performance.

The target variable for prediction is `RainTomorrow`.

## Dataset

The project uses the "Rain in Australia" dataset, contained in the `weatherAUS.csv` file. This dataset contains approximately 10 years of daily weather observations from numerous Australian weather stations.

It includes 23 attributes, such as:
- `MinTemp` / `MaxTemp`
- `Rainfall`
- `WindGustSpeed`
- `Humidity9am` / `Humidity3pm`
- `Pressure9am` / `Pressure3pm`
- `RainToday`
- `RainTomorrow` (Target Variable)

## Technologies Used

* **Python**
* **Pandas**: For data manipulation and analysis.
* **NumPy**: For numerical operations.
* **Scikit-learn**: For data preprocessing (imputation, scaling), model training, and evaluation.
* **Matplotlib & Seaborn**: For data visualization and exploratory data analysis.
* **Jupyter Notebook**: For interactive code development.

## Project Workflow

The notebook follows a structured approach to solve this classification problem:

1.  **Data Loading & Initial Exploration**: The `weatherAUS.csv` dataset is loaded, and initial inspections (`.head()`, `.info()`, `.shape`) are performed to understand its structure.
2.  **Data Cleaning & Preprocessing**:
    * Handling of missing values in both numerical and categorical columns using appropriate imputation strategies.
    * Encoding of categorical variables (like `Location`, `WindGustDir`, etc.) into numerical format.
    * Outlier detection and treatment.
3.  **Exploratory Data Analysis (EDA)**: In-depth analysis of univariate and bivariate data to understand distributions and relationships between variables.
4.  **Feature Engineering**:
    * The `Date` column is parsed to extract `Year`, `Month`, and `Day`.
    * Features and the target variable (`RainTomorrow`) are separated.
5.  **Train-Test Split**: The dataset is divided into training (80%) and testing (20%) sets to evaluate the model on unseen data.
6.  **Feature Scaling**: Numerical features are scaled to a common range to ensure that all features contribute equally to the model's training.
7.  **Model Training**: A Logistic Regression model is instantiated and trained on the preprocessed training data.
8.  **Model Evaluation**:
    * The model's performance is evaluated on the test set.
    * Key metrics such as **Model Accuracy**, **Confusion Matrix**, and a detailed **Classification Report** (including precision, recall, and F1-score) are analyzed.
    * The model is checked for overfitting and underfitting.

## How to Run This Project

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd <repository-directory>
    ```

2.  **Create a virtual environment (optional but recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required libraries:**
    Create a `requirements.txt` file with the following content:
    ```
    pandas
    numpy
    scikit-learn
    matplotlib
    seaborn
    jupyter
    ```
    Then, run the installation command:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

5.  Open and run the `Weather prediction using Logistic regression.ipynb` file to see the complete analysis.
