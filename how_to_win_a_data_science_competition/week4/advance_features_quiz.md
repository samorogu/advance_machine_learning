## Imagine that we apply X = PCA(n_components=5).fit_transform(data) and data has shape (5000, 53). What is the shape of X?
* (5, 53)
* **(5000, 5)**
* (5, 5000)
* (53, 5)

## To which data NMF is NOT applicable?
* Bag-of-words matrix
* **Standartized matrix** Standartized" means that every feature column has zero mean and unit variance. This implies that we have negative values and cannot apply NMF.
* One-Hot encoded feature

## Suppose we have 2 categorical features: f1 with A possible values and f2 with B possible values. How many values will their interaction have?

* Exactly A + B
* Exactly A * B
* **Less or equal to A * B** True. Sometimes some value (e.g. *a*) from A cannot be used with some value (eg *b*) from B. In this case, we have no change to see *ab* combination. If all value from A can be used with all values from B -- we will get A*B new possible values.
* max(A, B)

## Imagine we have 2 categorical features represented as integers: f1 with all values in range [0, 1000] and f2 with values in range [0, 100]. What is the correct way to build their interaction?

* f1 + f2 There are some problems. For example, if f1+f2=100: it is an interaction of 0 and 100, 100 and 0, or 90 and 10?
* f1.astype(str) + f2.astype(str) There is some problems. For example, "123": it is an d interaction of "1" and "23" or "12" and "3"?
* **f1.astype(str) + "_" + f2.astype(str)**
* (f1 + f2).astype(str)  It is essentially the same way as just f1+f2.


## What is a correct way to get t-SNE projection of train and test data?
* Apply t-SNE to the train and after that to the test.
* Apply t-SNE to the test first and after to train.
* **Apply t-SNE to concatenation of train and test and split projection back.** this the rigth way since train and test will projected in the same way.
* Doesn't matter, all variants will produce the same result.

## Is it possible to do t-SNE projection into 20-dimensional space?
* **Yes, why not.** You can do tSNE projection into arbitrary space.
* No, only 2-dim or 3-dim projections are possible.

