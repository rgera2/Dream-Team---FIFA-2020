# Dream-Team---FIFA-2020
# INTRODUCTION
We have a FIFA dataset in which there are few columns named - rating, release clause and wages. We assume that we do not have these variables in upcoming out of time datasets. These can be used in various formations like rating a player as a better performing player or moderate or not up to the mark player. Additionally, it can also translate into a player who should be sent an invite to some club gatherings, events etc. We built 2 models using Supervised Learning on Rating variables and we made it a classification problem by splitting this variable into 2 classes: greater than or equal to 70 and less than 70 as our potential club member or not. We chose 70 as our threshold as most of the major clubs have only players whose rating is greater than 70. In order to compete with them, we are inclined to have only those players having ratings greater than our threshold. Additionally, we have worked with our model results to predict the cost to investors for offering a club membership annually. Our second model utilizes predicted rating class obtained from our previous best classifiers instead of “actual rating" and here, and a combination of release_clause and annual wages as cost to investors as our dependent variable.

# Dataset
We used the FIFA 2019 and 2020 data from the Kaggle FIFA complete player dataset which contains 18k+ unique players and 100+ attributes extracted from the latest edition of FIFA. 
Training Data - FIFA 19,
Test Data - FIFA 20

# Analysis
Before building both the models, following steps were performed:
1. Data Cleaning - Selected relevant variables on the basis of dictionary definitions
2. Exploratory Data Analysis - Univariate and Bivariate
3. Feature Engineering

# Models
1. For Classification - Logistic Regression, KNN, Decision Tree, SVM (linear and radial)
2. For Regression - Linear model and Decision Trees

# Evaluation Metrics 
1. For Classification - Test Accuracy, AUC, F1 score, Precision-Recall curve
2. For Regression - RMSE and R-square

# Final Strategy
Final step was to make a strategy to pick players for our team keeping in mind:
1. Rating should be greater than 70 (means class 1)
2. Budget - 1 billion Euros and number of players around 30.

Firstly, we selected only the players who had ratings greater than threshold of 70. Number of players left - 5276

Secondly, we performed some analysis like the decile analysis of the cost to investors. We made some buckets each having approximately 30 players from the remaining pool and sorted those buckets based on cost to investors in descending order.

The best solution is to pick 8-10 core players from the top buckets and rest of the players from medium and low-valued buckets.
This decision can be easily made by the above analysis and it is up to the investors and team managers to decide that what kind of players they want in their team.
