# Credit Score Classification and Association Rule Mining in Python

## Project Overview

This project involves analyzing and modeling a large dataset of customer credit scores. The primary objectives include:

1. **Data Cleaning and Preprocessing:** Deep cleaning and outlier removal to ensure data quality.
2. **Handling Class Imbalance:** Addressing class imbalance using oversampling techniques.
3. **Machine Learning Modeling:** Building and evaluating machine learning models to classify credit scores, achieving significant accuracy and AUC metrics.
4. **Association Rule Mining:** Exploring the dataset for interesting relationships using the Apriori algorithm.

## Table of Contents

- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Handling Class Imbalance](#handling-class-imbalance)
- [Machine Learning Modeling](#machine-learning-modeling)
- [Association Rule Mining](#association-rule-mining)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Data Cleaning and Preprocessing

- **Outlier Removal:** Initially, the dataset was cleaned by removing outliers that could skew the analysis.
- **Missing Values:** Addressed any missing values by employing suitable imputation techniques.
- **Feature Engineering:** Created new features to enhance the model's predictive power.

## Handling Class Imbalance

The dataset exhibited significant class imbalance, which was addressed using oversampling techniques:

- **Oversampling:** Applied Synthetic Minority Over-sampling Technique (SMOTE) to balance the classes effectively.
- **Validation:** Ensured the balanced dataset did not lead to overfitting by using cross-validation techniques.

## Machine Learning Modeling

Several machine learning models were built and evaluated, including:

- **Logistic Regression**
- **Random Forest**
- **Gradient Boosting Machines**
- **Support Vector Machines (SVM)**

The models were assessed using the following metrics:

- **Accuracy:** Achieved an accuracy of 82%.
- **AUC (Area Under Curve):** Recorded an impressive AUC score of 95.6%.

## Association Rule Mining

Using the **Apriori algorithm**, interesting relationships between variables were explored. The key outcomes were:

- **Confidence:** Mined association rules with an average confidence level of 50%.
- **Support and Lift:** Evaluated the support and lift of the rules to ensure they were meaningful and actionable.

## Results

- **Classification Models:** Successfully built and tuned models to classify credit scores with high accuracy and AUC.
- **Association Rules:** Discovered several meaningful associations that could inform further business decisions.

## Conclusion

This project demonstrates a comprehensive approach to tackling a real-world credit score classification problem, from data cleaning to advanced machine learning and association rule mining. The insights derived could be valuable for financial institutions in assessing creditworthiness and discovering patterns in customer behavior.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
