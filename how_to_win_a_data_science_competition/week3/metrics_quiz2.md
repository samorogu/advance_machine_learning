## Suppose we solve a binary classification task and our solution is scores with logloss. What predictions are more preferable in terms of logloss if true labels are y_true = [0, 0, 0, 0].


* **y_pred = [0.5, 0.5, 0.5, 0.5]**
* y_pred = [0.4, 0.5, 0.5, 0.6]
* y_pred = [0, 0, 0, 1]

## Suppose we solve a regression task and we optimize MSE error. If we managed to lower down MSE loss on either train set or test set, how did we change Pearson correlation coefficient between target vector and the predictions on the same set?


* The correlation was also lowered.
* The correlation did not change.
* **Any behavior is possible.** We cannot monotonically relate MSE and Pearson correlation similarly to how e.g. R-squared monotonically related MSE,
* The correlation became larger.

## What would be a best constant prediction for a following multi-class classification task with 4 classes? The solution is scored with multi-class logloss. The number of objects of each class in train set is: 18, 3, 15, 24. Enter four comma separated values. Round each to two decimal places and use a leading zero before a fractional part (e.g. "0.50"; not ".5").

```counts = numpy.array([18, 3, 15, 24])
print(counts/counts.sum())
> [0.3  0.05 0.25 0.4 ]
```

## What is the best constant predictor for R-squared metric?
* Target mean divided by target variance
* 0.5
* **Target mean** As it is up to a constant is equal to MSE metri
* One minus target mean
* (Log of target mean) + 1

## Select the correct statements.
* **Optimization loss can different to target metric.** Sometimes we cannot use target metric as optimization loss. For example if our target metric is accuracy.
* Optimization loss is always different to target metric.
* Optimization loss is always the same as target metric.
* **Optimization loss can be the same as target metric.** Sometimes we can use target metric as optimization loss. For example if our target metric is MSE.

## Suppose the target metric is M1, and optimization loss is M2. We train a model and monitor its quality on a holdout set using metrics M1 and M2.

* **There is no definite relation between the best iterations for M1 score and M2 score.** There is no definite relation between the best iterations for M1 score and M2 score.
* If the best M1 score is attained at iteration N, then the best M2 score is always attained after N-th iteration.
* If the best M1 score is attained at iteration N, then the best M2 score is always attained also at the iteration N. It is not true in general. There are exceptions though. For example if M1 is MSE and M2 is R-squared.
* If the best M1 score is attained at iteration N, then the best M2 score is always attained before N-th iteration.
