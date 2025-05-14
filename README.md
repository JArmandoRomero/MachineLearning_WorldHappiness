# Predicting Happiness Score: The Role of Socio-Cultural and Political Factors in Regional Well-being

### Group 5  
**Members:** Britton Almy, Atul Gupta, Mary Proctor, Jarrod Romero Rangel  
**Course:** COSC522  
**University of Tennessee**  

## Overview

This project leverages the **World Happiness Report** dataset to predict happiness scores based on socio-cultural and political factors. By using machine learning techniques such as **Support Vector Regression (SVR)** and **Deep Learning Scalar Regression**, we aim to explore how various indicators—like GDP, social support, freedom, and mental health—impact regional well-being. The goal is to develop robust models that can forecast happiness scores while considering the complex interactions among multiple variables.

## Table of Contents

- [Introduction and Overview](#introduction-and-overview)
- [Data Sourcing and Preprocessing](#data-sourcing-and-preprocessing)
- [Methods](#methods)
- [Design](#design)
- [Related Work and Comparison](#related-work-and-comparison)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction and Overview

The **World Happiness Report** is a global survey that ranks countries based on perceived happiness. Each country's happiness score is derived using the **Cantril ladder** method, where respondents rate their life satisfaction on a scale from 0 to 10. Various socio-cultural and political factors, such as **GDP per capita**, **social support**, and **corruption perception**, have been identified as significant contributors to these happiness scores.

Our project explores these factors and builds predictive models to understand their relative importance in explaining regional well-being. We aim to identify key factors that influence happiness and predict the happiness scores of various countries using machine learning algorithms.

## Data Sourcing and Preprocessing

The dataset used for this analysis is sourced from the **World Happiness Report**. Key preprocessing steps include:

- **Data Cleaning:** Handling missing values, dropping rows with missing target values, and replacing missing features with means.
- **Feature Engineering:** Standardizing column names and creating derived metrics for deeper insights.
- **Data Transformation:** Encoding categorical variables (e.g., country) using **one-hot encoding**, and scaling numerical features with **StandardScaler** for consistency.
- **Exploratory Data Analysis (EDA):** Visualizations, such as correlation heatmaps and scatter plots, were generated to examine relationships between features.

## Methods

### Model Selection
We used the following regression models to predict happiness scores:

- **Linear Regression:** Simple and interpretable, but assumes a linear relationship between features and target.
- **Support Vector Regression (SVR):** Effective for high-dimensional data and non-linear relationships.
- **Random Forest Regression:** An ensemble method that can capture non-linear patterns through decision trees.
- **Gradient Boosting Machines (GBM):** Sequential decision trees that improve predictive accuracy.
- **Deep Learning (Scalar Regression):** Neural networks designed to capture more complex non-linear relationships.

### Evaluation Metrics
We evaluated model performance using:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **R-squared (R²)**

### Model Training & Hyperparameter Tuning
We performed model tuning for optimal performance and compared the results across different algorithms. Hyperparameters were adjusted to prevent overfitting and improve model generalization.

## Design

### Data Cleanup
- **Missing Values:** Rows with missing values were dropped, and missing numerical values were imputed with the mean.
- **Feature Scaling:** We applied **StandardScaler** to ensure consistent data scaling for machine learning models sensitive to feature magnitude differences.

### Feature Selection
- **Correlation Analysis:** We performed correlation analysis to identify highly correlated features and removed irrelevant ones.
- **f_regression:** A statistical method used for feature selection in regression models.

## Related Work and Comparison

Several studies have explored happiness prediction using both traditional and modern techniques. Early research primarily used **linear regression** (Helliwell et al., 2012), which focused on GDP, social support, and life expectancy. More recent studies have employed machine learning techniques like **Random Forests** and **SVR** (Kavakliotis et al., 2018), which can capture non-linear relationships.

Our project builds on this by also experimenting with **Deep Learning** models to explore deeper patterns in the data. We also consider a broader set of features (e.g., **internet access**, **mental health index**, **work-life balance**) that were not traditionally included in previous models. This approach aligns with recent trends (Munoz et al., 2021) suggesting that broader indicators provide a more holistic view of happiness.

### Key Studies:
1. **Helliwell et al. (2012)** - Focused on linear regression and factors like GDP and life expectancy.
2. **Kavakliotis et al. (2018)** - Applied **Random Forest** and **SVR** for predicting happiness.
3. **Trabucco et al. (2020)** - Introduced deep learning models for happiness prediction, exploring non-linear patterns.
4. **Munoz et al. (2021)** - Advocated for using diverse features such as internet access and mental health.

## Conclusion

In conclusion, this project demonstrated that machine learning models, especially **Random Forest** and **XGBoost**, are highly effective for predicting happiness scores. Additionally, deep learning models hold promise for capturing even more complex relationships as more detailed datasets become available. Our results emphasize the importance of incorporating a diverse set of socio-cultural and political features in happiness prediction models, as these can provide deeper insights into regional well-being.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to explore and contribute to the repository.
