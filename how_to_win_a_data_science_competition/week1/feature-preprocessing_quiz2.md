## Suppose we have a feature with all the values between 0 and 1 except few outliers larger than 1. What can help us to decrease outliers' influence on non-tree models?



* **Apply np.sqrt(x) transform to the data**
* **Apply np.log1p(x) transform to the data**
* **Apply rank transform to the features**
* **Winsorization**
* **MinMaxScaler**
* **StandardScaler**


## Suppose we fit a tree-based model. In which cases label encoding can be better to use than one-hot encoding?


* **When categorical feature is ordinal**
* **When we can come up with label encoder, that assigns close labels to similar (in terms of target) categories**
* **When the number of categorical features in the dataset is huge**


## Suppose we fit a tree-based model on several categorical features. In which cases applying one-hot encoding can be better to use than label-encoding?


* When the feature have only two unique values
* **If target dependence on the label encoded feature is very non-linear, i.e. values that are close to each other in the label encode feature correspond to target values that aren't close.**

## Suppose we have a categorical feature and a linear model. We need to somehow encode this feature. Which of the following statements are true?


* Label encoding is always better than one-hot encoding
* One-hot encoding is always better than label encoding
* **Depending on the dataset either of label encoder or one-hot encoder could be better**