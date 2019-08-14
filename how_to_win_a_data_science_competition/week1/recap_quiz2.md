## What back propagation is usually used for in neural networks?


* Select gradient update direction by flipping a coin
* **To calculate gradient of the loss function with respect to the parameters of the network**
* To propagate signal through network from input to output only
* Make several random perturbations of parameters and go back to the best one

## Suppose we've trained a RandomForest model with 100 trees. Consider two cases:

We drop the first tree in the model
We drop the last tree in the model
We then compare models performance on the train set. Select the right answer.


* In the case 1 performance will drop less than in the case 2
* **In the case 1 performance will drop more than in the case 2**
* In the case 1 performance will be roughly the same as in the case 2

## Suppose we've trained a GBDT model with 100 trees with a fairly large learning rate. Consider two cases:

We drop the first tree in the model
We drop the last tree in the model
We then compare models performance on the train set. Select the right answer.


* In the case 1 performance will drop more than in the case 2
* In the case 1 performance will drop less than in the case 2
* In the case 1 performance will be roughly the same as in the case 2

## Consider two cases:

We fit two RandomForestClassifiers 500 trees each and average their predicted probabilities on the test set.
We fit a RandomForestClassifier with 1000 trees and use it to get test set probabilities.
All hyperparameters except number of trees are the same for all models.

Select the right answer.


* The quality of predictions in the case 1 will be higher than the quality of the predictions in the case 2
* **The quality of predictions in the case 1 will be roughly the same as the quality of the predictions in the case 2**
* The quality of predictions in the case 1 will be lower than the quality of the predictions in the case 2

## What model was most probably used to produce such decision surface? Color (from white to purple) shows predicted probability for a point to be of class "red".

* k-NN
* Linear model
* Random Forest
* **Decision Tree**

## What model was most probably used to produce such decision surface?

* Linear model
* Decision Tree
* k-NN
* **Random Forest**