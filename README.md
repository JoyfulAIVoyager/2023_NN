# 2023_NN
## I. Project Title:

Neural Forecasting: Predicting Corporate Bankruptcy from Financial Indicators

## II. Project Introduction:

### Objective:

To design and implement a neural network model that can accurately predict the risk of corporate bankruptcy from given financial indicators

### Motivation:

Bankruptcies can have ripple effects across economies, affecting job markets, stock markets, and the general health of the financial system. Traditional statistical methods of predicting bankruptcy, while effective, might not capture the intricate relationships present in modern financial systems. Neural networks, with their ability to learn and generalize from complex datasets, offer an avenue for enhancing predictive accuracy. Given the advancements in deep learning and the increasing availability of financial data, this project seeks to explore the potential of neural networks in the realm of financial forecasting.

## III. Dataset Description:

### Source: 

#### [ Taiwanese Bankruptcy Prediction. (2020). UCI Machine Learning Repository. https://doi.org/10.24432/C5004D. ]
The dataset, sourced from the UCI Machine Learning Repository, contains financial attributes of Taiwanese companies from 1999 to 2009, and it's structured to assist in predicting the possibility of bankruptcy based on these financial attributes.


###  Features (Financial Attributes):

The dataset comprises 95 features financial attributes, representing different financial metrics that provide insight into various facets of a company's financial health. Some notable attributes include:

### Label (Bankruptcy):
Bankruptcy Status (1: Went Bankrupt, 0: Did not go bankrupt)

### Data Splitting
The data is divided into three sets and uploaded:

Training set (60%): Used to train our neural network model. (train_dataset.csv)

Validation set (20%): To tune the model parameters and prevent overfitting. (valid_dataset.csv)

Test set (20%): To evaluate the model's performance on unseen data. (test_dataset.csv)

