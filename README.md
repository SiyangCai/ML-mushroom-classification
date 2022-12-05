# Data Science project: mushroom classification
 
[This mushroom dataset](https://www.kaggle.com/datasets/uciml/mushroom-classification) (donated to UCI ML 27 April 1987) includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family Mushroom drawn from The Audubon Society Field Guide to North American Mushrooms (1981). Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. 

## Data Cleaning
* No missing values.
* Total number of 8,124 mushrooms, with 4,208 edible and 3,916 poisonous.
* 22 features that describe the attributes of the mushrooms.
* All features are categorical variables, which includes
 -

## Model Building
The target of this project is to using machine learning methods to help identify all the mushrooms in the dataset between edible and poisonous. Firstly, all of the features are transformed by one hot encoder. Then I have used three different models:
* Logistic Regression, 
* Support Vector Machine, 
* A Voting Classifier, which I thought should give a better result compared to one single model.

Best model performance (accuracy) will be searched under randomized gird seach regarding the hyper parameters. 10 Cross validations are performed.

## Model performance
Voting classifer does improve the accruracy but does not differ very much compared to other two models.
* Logistic Regression: 98.07%,
* Support Vector Machine: 98.28%,
* Voting Classifier: 98.35%.
