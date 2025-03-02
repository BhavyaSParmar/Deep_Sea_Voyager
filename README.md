# Deep_Sea_Voyager
Overview

This project performs an in-depth analysis of Sea Voyager survival data, focusing on data preprocessing, exploratory data analysis (EDA), and machine learning models to predict survival outcomes.

Data Preparation and Cleaning

Library Imports: Essential libraries such as pandas, numpy, seaborn, and matplotlib are imported for data manipulation and visualization.

Dataset Loading: The Titanic dataset (Titanic Survival.csv) is loaded into a Pandas DataFrame for analysis.

Handling Missing Values:

The Age column contains 177 missing values, which are replaced with 0.

The Cabin column contains numerous missing values, which are replaced with "No Cabin".

Memory Optimization:

Data types of categorical variables (Sex, Pclass, Parch, SibSp) are converted to categorical data types to reduce memory usage.

Exploratory Data Analysis (EDA)

Distribution Analysis: Various plots such as histograms and count plots are generated to analyze the survival distribution across different features.

Feature Engineering:

A function is implemented to extract title prefixes (e.g., Mr., Mrs., Miss) from passenger names.

Titles are mapped to standardized categories to enhance predictive modeling.

Correlation Analysis:

The correlation between different features and survival is explored using a heatmap.

Data Visualization

Survival Rate by Gender: A count plot is used to visualize the survival rates for males and females.

Survival Rate by Passenger Class: A bar plot is used to analyze survival differences across different passenger classes.

Age Distribution: A violin plot shows the distribution of ages for survivors and non-survivors.

Machine Learning Models

Data Splitting: The dataset is split into training and testing sets using train_test_split.

Feature Engineering: Additional preprocessing steps such as encoding categorical variables and scaling numerical features are applied.

Model Selection and Training:

Logistic Regression:

Trained on preprocessed data and evaluated using accuracy and classification reports.

Random Forest Classifier:

Uses 200 decision trees to classify survival outcomes.

Evaluated based on accuracy, precision, recall, and F1-score.

Performance Evaluation:

Accuracy, precision, recall, and confusion matrices are used to assess model performance.

Key Insights and Conclusion

Gender is a strong predictor: Women had a significantly higher survival rate than men.

Passenger Class Matters: First-class passengers had a higher probability of survival compared to second and third-class passengers.

Age has an impact: Younger passengers, particularly children, had higher survival rates.

Machine learning models successfully predict survival outcomes, with Random Forest providing better performance than Logistic Regression.

This project demonstrates a full end-to-end workflow of data preprocessing, exploratory data analysis, feature engineering, and machine learning modeling to analyze Titanic survival data.
