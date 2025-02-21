# PHASE 3 PROJECT
# Resevoir-Facies-Classification
Predicting reservoir rock facies using well log data with machine learning.

## Overview
The Reservior Facies Classification project aims to predict the reservoir rock facies using well log data. Accurate prediction of the rock facies is crucial in the oil and gas industry for reservoir characterization, helping to guide drilling and exploration decisions.

### Main Objective
To develop a machine learning model that classifies rock facies based on well log features, facilitating more informed geological interpretations and operational decision making.

### Specific Objectives
1. Develop a machine learning model to classify facies with high accuracy.
2. Enhance the accuracy of geological interpretations for improved exploration and production decisions.
3. Identify key features from the well log data that influence facies classification.

**Key Questions**    
1. What features from the well log data are most influential in afacies classification? 
2. Which machine learning model best captures the complex relationships within the geological data?
3. How can model predictions support better drilling decisions and reduce operational risks? 

## Methodology
This project follows a structured approach based on the CRISP-DM methodology, involving the following phases:

Business Understanding: The goal is to predict reservoir facies to assist with exploration and production decisions.

Data Understanding: Analyzing the dataset's features, identifying class imbalance, and understanding the relationship between variables.

Data Preparation: Preprocessing the dataset, including encoding categorical features and handling missing values.

Modeling: Building and comparing various machine learning models to predict facies.
Evaluation: Assessing model performance using metrics such as accuracy, precision, recall, F1-score.

Deployment: Summarizing findings and making recommendations for further exploration.

### Dataset Used
Features in the dataset:
Each well log contains the following features: Gamma Ray(GR) - Measures natural radioactivity of formations.

Resistivity Logging(ILD_LOG10) - Logs the electrical resistivity of rock formations.

Photoelectric Effect(PE) - Indicates mineral composition.

Neutron-Density Porosity(DeltaPHI) - Difference between neutron and density porosity.

Average Neutron-Density Pororsity(PHID) - Average neutron and density porosity.

Nonmarine-Marine Indicator(NM_M) - Distinguishes between marine and nonmarine environments.

Relative Position(RELPOS) - Represents the relative stratigraphic position within the reservoir.

Facies - Target variable

## Analysis Approach
#### 1. Univariate Analysis
Exploration of individual features to understand their distribution and how they relate to the target variable. This visualizations such as histogram, box plots summary statistics.

####  2. Bivariate Analysis
Examining relationship between each feature and the target variable. This helps identify correlation and patterns in the data. Scatterplots, heatmaps were used.

#### 3. Multivariate Analysis
Using techniques such as pairplots,and other dimensionality reduction methods to explore relationships between multiple variable simultaneously.

## Modeling
Several machine learning models were tested and compared for the classification task:
**Logistic Regression**: Baseline model with 53.25% accuracy.

**Decision Tree Classifier**: Improved model with 73.61% accuracy.

**Random Forest Classifier**: Best performing model with hyperparameter tuning achieving 81.33% accuracy.

## Evaluation
Model evaluation includes accuracy, precision, recall, F1-score. The Random Forest Classifiernmodel achieved an accuracy of 81.33% and performed well across all facies classes.

#### Performance Metrics:
Accuracy: 81.33%
Precision, Recall, F1 score: Evaluated across all facies.

#### Feature Importance:
Random Forest feature importance was analysed to show which features contributed most to the model's predictions.

## Tableau Visualizations 
Tableau was used to create interactive dashboards to visualize:
1. Distribution of well log data.
2. Class distributions and model predictions.
3. Feature importance and relationships between variables.
4. Insights into model performance across different facies.

## Key Findings
The Random Forest Classifier outperformed other models, achieving the highest accuracy.
SMOTE successfully mitigated class imbalance, improving model generalization.
Key features that contributed significantly to classification include **Gamma Ray(GR)**, **Resistivity(ILD_log10** and **Porosity**.

## Recommendations
Based on the model evaluation, the Random Forest model is recommended for use in predicting reservoir rock facies.
Future work should focus on collecting more data for rare facies classes to further improve prediction accuracy.
Implementation addditional geological features could potentially enhance the model's predictive power.