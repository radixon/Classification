# Objective

Create a predictive model that will determine the position of NBA players: Backcourt(B) or Frontcourt(F).

# Data Description

- The NBA dataset originated from [this](https://www.basketball-reference.com/leagues/NBA_2020_per_game.html) basketball-reference page.
- Glossary for terms can be found [here](https://www.basketball-reference.com/about/glossary.html). (Note: This data file contains per game averages)
- **Edit:** Positions (Pos) has been simplified into two classifiers: [Frontcourt (F) and Backcourt (B)](https://www.rookieroad.com/basketball/the-court/front/).

# Models

There were three models used with various hyperparameters to before chosing a model to run against the test data.

## Logistic Regression

Logistic regression models work best on binary target variables, and data that doesn't have many missing values or outliers.  This makes this a very strong option for this dataset.

## Random Forest

Random forest models works well with categorical or continuous target variables.  Random forest works well with messy data, such as missing values and outliers.  With that said, random forest models generally aren't the best models for relatively complex or novel problems.


## Gradient Boosting Classifier

Boosting models are very similar to random forest models.  The main difference being random forest models use independent trees; whereas, boosted models iteratively builds weak models where each model learns from the previous model's mistakes.  As such, boosted models works well with categorical or continuos target variables, and messy data.

# Key Findings

All models showed predictive power.  With this specific dataset, the boosted model had the most predictive power.
![image](https://github.com/radixon/Classification/assets/59415488/03f658e1-64c9-43d4-8d65-ca7f26b56582)


# Plan of Action

With the boosted model performance, more data should be used.  While the accuracy, precision, and recall numbers are strong, test should be conducted on a larger dataset before the results can be considered reliable.
