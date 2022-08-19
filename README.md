# IPL-cricket-score-prediction

The purpose of the project is to build a regression model to predict first innings score of the cricket match based on runs scored by teams in previous matches.

The IPL score dataset was obtained from Kaggle. It consists 76000 records and 15 columns representing venue of the match, batting team, total score of match, bowling team, name of batsman and bowler and runs scored for each bowling delivery etc.

Performed preprocessing of data like removing certain variables like 'mid','venue','batsman','bowler','striker','non-striker' deemed redundant in predicting the score. Also removed records for IPL teams which played in the past but not playing in the current tournament. Performed one hot encoding for nominal categorical variables in the dataset.

Obtained a time series train test split (records corresponding to years 2016 as training set and records corresponding to year 2017 as test set) and built a  ridge regression model. The optimal alpha for ridge was obtained by hyper parameter searching for a range of alpha values using GridSearchCV. The model was evaluated using MAE, MSE and RMSE metrics.



