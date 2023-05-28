# sentiment-analysis-on-company-reviews
The goal of this project is to predict the sentiment of company reviews left by customers. The target is a star rating between 1 and 5. 

## About the dataset
The dataset consists of 100,000 reviews collected from Trustpilot and spans over 40 different companies. The samples are split according to: 60% train, 10% public leaderboard and 30% private leaderboard.

## Data Preprocess
In the data preprocessing, HTML tags were removed from the input text and replaced with an empty string. Emojis were converted to their textual representation. Used regular expressions(re) package to eliminate stop words and retain important words.

## Model Implementation
### Vectorization
* Scaled the data: Applied a scaling technique (Standardization) to ensure all features have a similar scale or distribution.
* Added reviewed texts length as a new feature: Calculated the length of each review text and added it as a new feature/column in the dataset.
* Transformed the data into a sparse matrix format: Converted the dataset into a sparse matrix representation, which is a memory-efficient way of storing large matrices with mostly zero values.
### Model Fitting
Applied Logistic Regression, Multi-Layer Perceptron Classifier, and Random Forest models.
### Evaluation
The highest sentiment prediction accuracy is 86% from the multi-layer perceptron classifier.
