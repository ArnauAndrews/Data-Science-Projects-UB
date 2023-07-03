# News Classification (HuffPost)

![HuffPost svg](https://github.com/ArnauAndrews/Data-Analytics-Projects-Ubiqum/assets/132329252/d4e774be-c68d-4c66-9464-bc118095eef9)

## Abstract 
The project involved several key steps. First, we trained a Naive-Bayes model using a dataset of 200,000 news headlines, exploring different alpha values to optimize its performance. Then, we evaluated the model's accuracy by applying it to new data obtained through web scraping using Beautiful Soup. Finally, we iteratively refined the model by finding the best alpha parameter, aiming to strike a balance between underfitting and overfitting, and improve its predictive capabilities for news article classification.

## Table of Contents
- [Context](#context)
- [Variables](#variables)
- [Objective](#objective)
- [Approach and Models Used](#approach-and-models-used)
- [Web Scraping](#web-scraping)
- [Findings & Conclusions](#findings--conclusions)
- [Applications and Next Steps](#applications-and-next-steps)

## Context
This project focuses on classifying news articles based on their headlines using the Naive-Bayes algorithm. The dataset used contains around 200,000 news headlines from the year 2012 to 2018 obtained from HuffPost. The goal is to create a model that can identify the category of news articles or analyze the language used in different news articles.

## Variables
The dataset is in JSON format and includes the following keys:

- `Category`: Represents the category of the article, which is the variable we want to estimate.
- `Headline`: The headline of the HuffPost news article.
- `Authors`: Indicates the authors of the articles.
- `Link`: Provides the URL of the news article.
- `Short_description`: Gives a summary of the article.
- `Date`: Represents the date of the article.

## Objective
The main tasks involved in this project are as follows:

1. Create a **multiclass classification model** that can identify the categories: WELLNESS, PARENTING, TRAVEL, BUSINESS, and SPORTS.
2. Perform **web scraping** of article headlines from the web in the mentioned categories, retrieving more than 20 headlines per category.
3. Apply the trained **Naive-Bayes model** to check its performance with current articles.
4. The model building approach involves:
   - Reading the JSON file and converting it to a Pandas DataFrame.
   - Performing text preprocessing techniques as covered in module 3.
   - Applying Naive-Bayes by analyzing different values of the "Alpha" parameter.
   - Evaluating the model's performance and commenting on the results.
5. The web scraping steps include:
   - Collecting more than 20 article headlines for each category (WELLNESS, PARENTING, TRAVEL, BUSINESS, and SPORTS).
   - Applying TF-IDF Vectorizer to the headlines.
   - Making predictions using the trained model.
   - Evaluating and commenting on the results.

## Approach and Models Used
The project follows the following approach:

1. **Data preprocessing:** The dataset is converted into a Pandas DataFrame, and text preprocessing techniques are applied.
2. **Model training**: A **Naive-Bayes** algorithm is used for multiclass classification, with different values of the "Alpha" parameter tested.
3. **Model evaluation:** The trained model's performance is evaluated using precision, recall, and F1-score for each category, as well as the average precision.
4. **Web scraping:** Additional headlines are collected for each category from the web using **BeautifulSoup**
5. **Applying the model:** The trained model is applied to predict the categories of the new articles.
6. **Hyperparameter tunning:** Different values of the "Alpha" parameter are analyzed during model training to find the best balance between overfitting and underfitting. By evaluating the model's performance with different "Alpha" values, we choose the one that provides the best results in terms of precision, recall, and F1-score for each category, as well as the average precision which is 1.
7. **Evaluation** of the model's performance with new articles: The performance of the model is analyzed, considering precision and recall for each category.

## Web Scraping
Web scraping is performed to collect more article headlines for each category. This helps to expand the dataset and evaluate the model's performance on current articles. TF-IDF Vectorizer is then applied to the scraped headlines, and predictions are made using the trained model. The results are evaluated and commented on.

![Unknown](https://github.com/ArnauAndrews/Data-Analytics-Projects-Ubiqum/assets/132329252/ceb23f70-e53e-4dd6-9ef3-b3abb69cd01a)

## Findings & Conclusions
- The model achieves an overall accuracy of 60% in correctly classifying articles, which is higher than the No Information Rate (NIR) of 20%.
- The category with the highest predictive capacity is *Travel*, with a precision of 0.65 and a recall of 0.80.
- The category with the lowest predictive capacity is *Business*, with a precision of 0.64 and a recall of 0.326.
- To improve the model, it is recommended to test it with more articles and train it with more detailed keyword features for categories with lower predictive capacity (Business, Parenting, and Sports).
- Despite some categories having lower accuracy, the model provides significant value in classifying Travel and Wellness articles, and its classifications can be confidently used in those categories.

## Applications and Next Steps
The developed model has various applications, such as automated article categorization, content recommendation systems, or analyzing language patterns in news articles. The model's performance can be further improved by incorporating more training data, experimenting with different feature engineering techniques, or trying advanced machine learning algorithms. 
