##Select true statements about n-grams


* N-grams always help increase significance of important words
* Levenshteining should always be applied before computing n-grams
* **N-grams can help utilize local context around each word**  n-grams encode sequences of words
* **N-grams features are typically sparse** n-grams count occurrences of words and not every word will be found in every document


## Select true statements.

* Meaning of each value in BOW matrix is unknown.
* You do not need bag of words features in a competition if you have word2vec features.
* **Semantically similar words usually have similar word2vec embeddings.**
* **Bag of words usually produces longer vectors than Word2vec**


## Suppose in a new competition we are given a dataset of 2D medical images. We want to extract image descriptors from a hidden layer of a neural network pretrained on the ImageNet dataset. We will then use extracted descriptors to train a simple logistic regression model to classify images from our dataset.

* We consider to use two networks: ResNet-50 with imagenet accuracy of X and VGG-16 with imageNet accuracy of Y (X < Y). Select true statements.
* **It is not clear what descriptors are better on our dataset. We should evaluate both.**

* With one pretrained CNN model you can get only one vector of descriptors for an image.Incorrect. With one CNN you can get different descriptors from different layers.
* Descriptors from ResNet 50 will always be better than the ones from VGG-16 in our pipeline.Incorrect. Although, ResNet50 shows better performance on Imagenet, this depends on the a specific dataset and a specific task.
* Descriptors from ResNet-50 and from VGG-16 are always very similar in cosine distance.his depends on the a specific dataset and a specific task.
* For any image descriptors from the last hidden layer of ResNet-50 are the same as the descriptors from the last hidden layer of VGG-16.Moreover it is hard to come up with an image that will have the same descriptors in both networks.


## Data augmentation can be used at (1) train time (2) test time

* **True, True** Data augmentation can be used (1) to increase the amount of training data and (2) to average predictions for one augmented sample.
* False, True
* True, False
* False, False