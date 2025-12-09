#  Advanced Computational Physics CW2- Machine Learning VS Neural Networks
by up2107120

### LICENSE:
MIT License — see LICENSE file.

### TASK:
Pick a dataset of our choosing and use a traditional Machine Learning approach on it. Then on the same data, use a modern Neural Network approach to the data and compare results.

### DATASET CHOSEN:
Space Missions (https://www.kaggle.com/datasets/sameerk2004/space-missions-dataset)

### DESCRIPTION:
For my ACT coding project 2 the aim is to use a chosen dataset to develop, train and test a machine learning alogrithm of our choice; and then compare this to the output of a Neural Network which we also program, train and test on the same dataset. Being an Physics, Astrophysics and Cosmology student I have chosen a dataset called 'Space Mission data' from Kaggle (found at https://www.kaggle.com/datasets/sameerk2004/space-missions-dataset). This dataset has columns for mission type, date of launch, mission target, cost, crew size etc and will be used to train a gradient boost regressor machine learning alogorithm. Following the Scikit algorithm cheat sheet I decided my dataset wasn't a catagory set but was rather a quantity of discrete data points, leading me to looking at regression models until I decided upon the Gradient Boost regressor. 

Following the pipeline of creating a gradient boost regressor I scaled, augmented, engineered and improved on many of the features from the dataset in order to highlight and create new links that previously weren't shown or were very supressed in the standard data. This was then enhanced by gridsearching the results to find the most optimum hyperparameters for the gradient boost, which could then be trained and tested again on the augmented dataset, producing a gradient decent tree diagram as well as a feature importance plot highlighting the importance of the new scaled relations in the dataset. 

After printing the outputs of the gbr, I started on a Neural Network called a Multi Layer Perceptron for which my tabular data would be suited. This required the transforming of my dataset into columns and then into pytorch tensors to preform splits, data loading and defining of the neural network model. Once the pipeline was built for the MLP, I could then optimise using the ADAM optimiser and later on the optuna import which much like a gridsearch, performs my NN given a number of epochs a given number of times, each time changing my hyperparameters fine tuning them until the output is optimal. Once this has run, I can plot an 'accuracy vs epoch' scatter chart to ensure I am not overfitting my data or wasting GPU and CPU processing power.

The results of the gradient boost regressor and Multi layer perceptron are then comapred against each other and their results analysed. 
