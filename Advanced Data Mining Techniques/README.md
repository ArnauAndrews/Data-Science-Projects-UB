Access the full project on the following link: **https://rpubs.com/ArnauAndrews/1059081**

# Wine Classification using Factor Analysis and Linear Discriminant Analysis

## Table of Contents
- [Introduction](#introduction)
- [Workflow](#workflow)
- [Presentation](#presentation)
- [Findings and Conclusions](#findings-and-conclusions)

## Introduction
This project focuses on classifying wines based on their characteristics using Factor Analysis (FA) and Linear Discriminant Analysis (LDA).

## Workflow
1. Data preprocessing: The wine dataset is loaded and cleaned by handling missing values and outliers.
2. Exploratory Data Analysis (EDA): The dataset is analyzed to gain insights into the wine characteristics and their relationships.
3. Factor Analysis (FA): FA is performed to identify underlying factors in the dataset that explain the variation in wine attributes.
4. Feature Selection: The important factors identified through FA are selected as input features for classification.
5. Model Development: Several classification models, such as Decision Tree, Random Forest, and Logistic Regression, are trained using the selected features.
6. Model Evaluation: The performance of each model is evaluated using appropriate evaluation metrics, such as accuracy, precision, recall, and F1-score.
7. Linear Discriminant Analysis (LDA): LDA is applied to further enhance the classification accuracy by maximizing the separation between wine classes.
8. Random Forest Model: A new model using the Random Forest algorithm is trained on a new training dataset and evaluated on a new testing dataset.
9. Evaluation of Confusion Matrix: The performance of the Random Forest model is compared to the previous LDA model in terms of accuracy and sensitivity for minority classes.

## Presentation
The project findings and methodology were presented in a visually appealing presentation, including the following sections:
- Introduction: Overview of the wine classification problem and its importance.
- Data Analysis: Key insights obtained from the exploratory data analysis.
- Factor Analysis: Explanation of the factor analysis technique and its application to the wine dataset.
- Model Development: Description of the classification models used and their performance evaluation.
- Linear Discriminate Analysis: Insight into how LDA was employed to improve classification accuracy.
- Random Forest Model: Details of the new model trained using the Random Forest algorithm.
- Evaluation of Confusion Matrix: Comparison of the Random Forest model with the previous LDA model.

## Findings and Conclusions
Based on the analysis performed, the project yielded the following findings and conclusions:

### Factor Analysis (FA)
- In factorial analysis, if two variables have large loadings (high correlations) for the same factor, it can be inferred that those variables share some underlying characteristic or property that is being captured by that factor.
- In this case, Factor 1 represents the common characteristics of citric.acid found in certain types of red wines, such as those with high citric acid content.
- On the other hand, Factor 2 is associated with the characteristics of density (density), which could be determined by the amount of sugar and alcohol present in other types of red wines, such as those with high sugar and alcohol content.
- We could name these factors as "dry red wines" (Factor 1) and "sweet red wines" (Factor 2).

### Linear Discriminant Analysis (LDA)
The LDA model has adequately segmented the observations based on the predicted class. In the plot, we can see that the three categories of the predicted label are clearly separated and distinguishable by different colors. This indicates that the LDA model has successfully captured the underlying structure and patterns in the data related to the class variable.

### Random Forest Model
The Random Forest model has slightly better accuracy than the previous LDA model, with an accuracy of 0.8526, indicating higher accuracy.

Additionally, this model has better sensitivity for the minority class "Low" compared to the previous LDA model. However, the sensitivity for the "Good" class remains low in the Random Forest model, indicating that there is still room for improvement in the classification of different wine categories. Overall, the Random Forest model is a better choice for accuracy in classifying minority observations compared to the LDA model.


For a detailed understanding of the project and the code implementation, please refer to the project documentation and the associated code files.

