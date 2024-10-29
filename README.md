Scrabble Player Rating Prediction
This project was developed as part of the CS 559: Machine Learning Fundamentals and Applications course. The goal was to predict player ratings in online Scrabble games based on game metadata using various machine learning models. Our team participated in Kaggle’s Scrabble Player Rating competition and aimed to achieve high accuracy in predicting player ratings.

Project Overview
The project focuses on predicting player rankings on the Woogles.io platform, which hosts Scrabble games. The data consists of metadata from several thousand games played against AI, with detailed turn-by-turn actions. Using a variety of models, we sought to minimize the Root Mean Square Error (RMSE) of our predictions.

Dataset
The dataset provided by Kaggle includes four CSV files:

games.csv: Metadata about each game, such as who went first and the time controls.
turns.csv: Turn-by-turn data for each game, including points scored.
train.csv: Contains final scores and ratings for each player as of before the game.
test.csv: Similar structure to train.csv, used for testing model predictions.
Approach and Strategy
The dataset contained both categorical and numerical features. We handled missing values and noted that many players had played multiple games. This helped us understand that ratings likely did not fluctuate drastically in short spans. The team experimented with different preprocessing techniques and merged our findings to achieve the best results.

Models Implemented
Bayesian Ridge Regression - RMSE: 138.71
Linear Regression - RMSE: 129.07
Linear Regression with Stacking - RMSE: 127.58
XGBoost - RMSE: 127.01
Decision Tree Regressor - RMSE: 126.26
Multi-Layer Perceptron Classifier - RMSE: 122.72
Random Forest Classifier - RMSE: 185.83
The Linear Regression model with stacking and the Multi-Layer Perceptron achieved the best RMSE scores.

Results
Our final RMSE score was 175.9548, ranking our team 200th on the private leaderboard on the day of submission.

Conclusion
The Linear Regression with Stacking approach was effective for this regression task, given the structure of the dataset and the limited variation in player ratings. The project provided valuable insights into the challenges of categorical and numerical data preprocessing for machine learning tasks.

Team
Praneeth Gubba
Sahithh Gudiyella
Hemil Patel
Rocco Vaccone
License
This project is for educational purposes as part of the CS 559 course.

