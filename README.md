# Fall 2018 EE 461P Final Project
## Kaggle Expedia Hotel Recommendations Competition
  
The competition can be found [here](https://www.kaggle.com/c/expedia-hotel-recommendations)  
  
Group Members:  
* Andriy Dashko  
* Emil Häglund  
* Wesley Klock  
* Genki Oji  

## File descriptions
### ExpediaPreprocessing.ipynb
This notebook contains code that we wrote for preprocessing data. The original data consists of 37 million rows which represent 1.2 million users, so we decided to downsample to 10 thousand users, which resulted in about 320 thousand rows. In this downsampled dataset, we extracted useful features, removed noisy data created by travel agents, and filled in missing values.

### Expedia_Modeling.ipynb
This notebook performs PCA to select features to use in our models. We also evaluate a baseline model in which the 5 most common hotel clusters are used to predict users' preferred clusters. Lastly, we define the other models that we will use for our predictions.

### Expedia_Modeling_2.ipynb
This notebook uses models including SVMs, Factorization Machine, XGBoost, and Naive Bayes to predict user preferred clusters and outputs scores for each.

### results.ipynb
This notebook includes all of the results from our models using our downsampled testing and training sets and displayes them in graphical form.