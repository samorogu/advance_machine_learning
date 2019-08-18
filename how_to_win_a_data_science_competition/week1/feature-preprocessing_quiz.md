
## What type does a feature with values: [‘low’, ‘middle’, ‘high’] most likely have?

* Datetime
* Coordinates
* Text
* **Ordinal (ordered categorical)**
* Numeric
* Categorical

## Suppose you have a dataset X, and a version of X where each feature has been standard scaled. For which model types training or testing quality can be much different depending on the choice of the dataset?


* GBDT
* **Linear models**
* **Neural network**
* Random Forest
* **Nearest neighbours**

## Suppose we want to fit a GBDT model to a data with a categorical feature. We need to somehow encode the feature. Which of the following statements are true?


* **Depending on the dataset either of label encoder or one-hot encoder could be better**
* One-hot encoding is always better than label encoding
* Label encoding is always better to use than one-hot encoding

## What can be useful to do about missing values?

* **Replace them with a constant (-1/-999/etc.)**
* **Nothing, but use a model that can deal with them out of the box**
* **Impute with a feature mean**
* Impute with feature variance
* Apply standard scaler
* **Remove rows with missing values**
* **Reconstruct them (for example train a model to predict the missing values)**