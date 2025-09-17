# Medical Insurance Cost Prediction using Linear Regression

## Project Overview

This project aims to predict individual medical insurance costs based on a number of personal attributes. A **Linear Regression** model is developed to understand how factors like age, smoking habits, and BMI influence insurance charges. The entire project, from data exploration to model evaluation, is documented in the `Medical insurance Prediction using linear Regression.ipynb` Jupyter Notebook.

## Dataset

The project uses the `insurance.csv` dataset, which contains personal and health-related data for a number of individuals.

### Key Features:
* **age**: Age of the primary beneficiary.
* **sex**: Gender of the beneficiary (male/female).
* **bmi**: Body mass index, providing an understanding of body weight relative to height.
* **children**: Number of children covered by health insurance.
* **smoker**: Whether the person is a smoker (yes/no).
* **region**: The beneficiary's residential area in the US (northeast, northwest, southeast, southwest).
* **charges**: The individual's medical costs billed by the health insurance (this is the **target variable**).

## Technologies Used

* **Python**
* **Pandas**: For data loading and manipulation.
* **NumPy**: For numerical computations.
* **Scikit-learn**: For data preprocessing, model training, and evaluation.
* **Matplotlib & Seaborn**: For data visualization and exploratory data analysis.
* **Jupyter Notebook**: As the development environment.

## Project Workflow

The project follows a systematic approach to build and evaluate the prediction model:

1.  **Data Loading & Inspection**: The `insurance.csv` dataset is loaded, and its structure, data types, and statistical summary are examined.
2.  **Data Preprocessing**:
    * Categorical features (`sex`, `smoker`, `region`) are converted into numerical format using one-hot encoding to make them suitable for the regression model.
3.  **Exploratory Data Analysis (EDA)**:
    * The distribution of the target variable (`charges`) is analyzed.
    * Visualizations such as histograms and scatter plots are used to explore the relationships between different features and the insurance charges.
4.  **Data Preparation**: The dataset is split into features (X) and the target variable (y).
5.  **Train-Test Split**: The data is divided into a training set and a testing set to evaluate the model's performance on unseen data.
6.  **Model Training**: A `LinearRegression` model is instantiated and trained on the training dataset.
7.  **Model Evaluation**:
    * The model's performance is assessed using the **R-squared (R²)** metric on both the training and testing data to check for goodness of fit and potential overfitting.
    * The model is used to make predictions on new, unseen data to demonstrate its practical application.

## How to Run This Project

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd <repository-directory>
    ```

2.  **Create a virtual environment (recommended):**
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

5.  Open and run the `Medical insurance Prediction using linear Regression.ipynb` file.
