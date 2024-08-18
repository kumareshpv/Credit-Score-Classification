# Credit Score Classification and Association Rule Mining in Python

## Project Overview

This project involves the classification of credit scores and the mining of association rules using a dataset containing credit-related information of customers. The project covers a broad range of tasks, including data cleaning, preprocessing, exploratory data analysis (EDA), correlation analysis, handling class imbalance, building multiple machine learning models, and mining association rules.

### Dataset

- **Source:** [Credit Score Classification Dataset on Kaggle](https://www.kaggle.com/datasets/parisrohan/credit-score-classification)
- **Size:** 100,000 customer records with various features related to credit behavior.

## Table of Contents

- [Group Members](#group-members)
- [Installation](#installation)
- [Importing Libraries](#importing-libraries)
- [Data Preprocessing](#data-preprocessing)
  - [Data Cleaning](#data-cleaning)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Correlation Analysis](#correlation-analysis)
- [Handling Class Imbalance](#handling-class-imbalance)
- [Machine Learning Modeling](#machine-learning-modeling)
- [Association Rule Mining](#association-rule-mining)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Group Members

1. **Kumaresh Pendiyala Venkatesh** - A20542224
2. **Sannidhi Rao Ambaragonda** - A20550030
3. **Sonali Sahu Patel** - A20539250
4. **Sumanth Vuppu** - A20540921

## Installation

To run this project locally, ensure you have Python installed. You can install the required packages by running:

```bash
pip install -r requirements.txt
```

## Importing Libraries

A comprehensive list of libraries was imported to support data manipulation, visualization, model building, and evaluation, including:

- `pandas`, `numpy` for data handling
- `matplotlib`, `seaborn` for visualization
- `scikit-learn` for machine learning models
- `mlxtend` for association rule mining
- `imblearn` for handling class imbalance

## Data Preprocessing

### Data Cleaning

The data cleaning process involved several key steps:

- **Removing Duplicates:** All duplicate records were identified and removed.
- **Handling Missing Values:** Missing values were imputed using appropriate strategies to maintain data integrity.
- **Correcting Invalid Characters:** Columns with invalid characters (e.g., '_') were identified and corrected.
- **Outlier Removal:** Outliers were detected and removed to ensure that they did not adversely affect the analysis.
- **Feature Engineering:** New features were created to enhance the predictive capabilities of the models.

### Exploratory Data Analysis

- **Descriptive Statistics:** Generated summary statistics to understand the distribution and key characteristics of the data.
- **Visualizations:** Used histograms, box plots, and bar charts to explore data distributions, relationships, and potential trends.

### Correlation Analysis

- **Correlation Matrix:** A correlation matrix was generated to identify relationships between features, helping in the selection of features for model building.
- **Heatmaps:** Visualized the correlation matrix using heatmaps to easily identify strong positive or negative correlations.

## Handling Class Imbalance

The dataset exhibited a significant class imbalance, which was addressed using the following technique:

- **SMOTE (Synthetic Minority Over-sampling Technique):** Applied SMOTE to balance the classes effectively, followed by cross-validation to avoid overfitting.

## Machine Learning Modeling

A total of **10 machine learning models** were built, trained, and evaluated, including:

1. **Logistic Regression**
2. **K-Nearest Neighbors (KNN)**
3. **Decision Tree Classifier**
4. **Random Forest Classifier**
5. **Support Vector Machines (SVM)**
6. **Naive Bayes**
7. **Gradient Boosting Machines (GBM)**
8. **XGBoost**
9. **LightGBM**
10. **AdaBoost**

### Model Evaluation Metrics:

- **Accuracy:** The highest accuracy achieved was 82%.
- **AUC (Area Under Curve):** The top-performing model recorded an AUC score of 95.6%.
- **Confusion Matrix:** Used to evaluate the performance of the classification models.
- **Precision, Recall, and F1-Score:** Additional metrics were computed to provide a deeper understanding of model performance.

## Association Rule Mining

Using the **Apriori algorithm**, association rules were mined to uncover interesting relationships within the data:

- **Support, Confidence, and Lift:** These metrics were used to evaluate the strength and relevance of the discovered rules.

### Example Association Rules:

1. **Rule:** `(Interest_Rate [2.28 to 3.42]) → (Credit_Score_Good)`
   - **Support:** 10.62%
   - **Confidence:** 55.8%
   - **Lift:** 1.156
   - **Interpretation:** Customers with an interest rate between 2.28 and 3.42 are likely to have a good credit score.

2. **Rule:** `(Credit_Score_Good) → (Num_Credit_Card [4.0 to 5.0])`
   - **Support:** 10.1%
   - **Confidence:** 56.8%
   - **Lift:** 1.757
   - **Interpretation:** Customers with a good credit score tend to have between 4 and 5 credit cards.

## Results

- **Classification Models:** The best model achieved an accuracy of 82% and an AUC of 95.6%.
- **Association Rules:** Several meaningful associations were discovered, which can provide actionable insights into customer behavior and creditworthiness.

## Conclusion

This project successfully demonstrates the application of advanced data cleaning, machine learning, and association rule mining techniques to solve a real-world credit score classification problem. The insights derived from this project could be invaluable for financial institutions in assessing creditworthiness and understanding customer behavior patterns.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
