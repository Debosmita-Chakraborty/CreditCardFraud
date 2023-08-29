# CreditCardFraud
Detecting fraudulent credit card transactions in anonymized dataset using Supervised Machine Learning (Classification)

## Context
Finance meets crime fighting! Two fascinating subjects combined, with the additional challenge of an anonymized dataset, made this project a thrill to work on. I found it incredibly motivating to work on something that has such a real-world impact- losses from financial fraud affect both large financial institutions and ordinary people.

Now, about the project. I performed undersampling on the highly imbalanced dataset (turns out an overwhelming percentage of people are nice, honest folks!), removed extreme outliers and did some clustering using t-SNE and PCA before finally building some classification models (mainly Logistic Regression and Support Vector Machine or SVM) to predict if a transaction is fraudulent or genuine. I analysed the performance of the models using metrics like precision, recall, AUC/ROC graphs for comparision and identification of the best performing models.

## Skills
Skills shown:

 *   Data cleaning (e.g. outlier removal)
 *   Dealing with imbalanced data
 *   Principal Component Analysis (PCA) and t-SNE
 *   Implementing Supervised Machine Learning models (Classification), using GridSearch

New Skills Learnt:

 *   Dealing with anonymized data
 *   t-SNE
 *   A deeper understanding of AUC/ROC curves

## Process

*    I first performed some intitial EDA to find the extent to which the data is imbalanced (over 99% was non-fraud), then scaled the unscaled features using RobustScaler.
*    Next I performed shuffling and undersampling of the majority class (non-fraud transactions) to bring the numbers down to a 50-50 split between fraud and non-fraud transactions.
*    I analysed this subsampled dataset's correlation matrix to find which features are related and can impact the target variable (since we don't know what the features are, data has been anonymized for privacy) either by positive or negative correlation
*    To improve accuracy I removed the extreme outliers from highly correlated features that may mislead our analysis, followed by t-SNE and PCA
*    Then I implemented Logistic Regression and SVM and analysed their performance metrics in depth. I then used GridSearch to find the optimal parameters for 4 classification models - Logistic Regression, K Nearest Neighbors, Support Vector Machine and Decision Tree - to compare their performance by visualising the AUC/ROC curve
*    Some problems that I faced include dealing with anonymized data and consolidating 4 separate ROC curves in a single graph(shoutout to <a href='https://www.kaggle.com/code/janiobachmann/credit-fraud-dealing-with-imbalanced-datasets'>Janio Bachmann's notebook</a>!)
  
## Sources
* https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
