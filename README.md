I have chosen a Space Mission data set that has information such as flight time, crew numbers, cost and launch vehicles to name a few. Following the Scikit algorithm cheat sheet I decided my dataset wasn'ta catagory 
set but was a quantity set rather than labeled data. This led me to looking a regression models until I decided upon the Gradient Boost regressor. This was for a few main reasons such as my smallish row count (500 rows)
as well as the non-linear relations between mixed type features such as cost and distance to different target types, which do not scale linearly. Originally also my data was not scaled which wasn't an immediate problem for feature importance but was
later changed anyway when new engineered features were introduced. Finally gbr are also fine tunable allowing me to perform a gradient search for model parameters on it, and then retrain my model on these hyperparams
to get the best model fit possible. 
