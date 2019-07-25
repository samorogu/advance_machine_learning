## Which of the following is true about word2vec model?
* It requires human-defined semantic relations between words.
* **It requires some text corpora for training.**
*  It has one trainable parameter per word.
* It's outputs (predictions) are linear functions of inputs.
* It uses convolutional layers and pooling.

## How can you train word2vec model?
* **By learning to predict omitted word by it's context.**
* ** By learning to predict context (neighboring words) given one word.**
* ** By minimizing crossentropy (aka maximizing likelihood).**
* By changing order of words in the corpora.
* By minimizing distance between human-defined synonyms and maximizing distance between antonyms.
* **By applying stochastic gradient descent.**

## Here's an online demo of word2vec model. Let's use it to find synonyms for rare words. Don't forget to choose English GoogleNews model. Which of the following words is in top 10 synonyms for "weltschmerz".
* worldbuilding
* decrystalization
* **despair**
* big_bang

## Which of the following is an appropriate way to measure similarity between word vectors v1 and v2? (more = better)

* ** cos(v1,v2) **
* ** -||v1 - v2|| **
*  ||v1 - v2||
* sin(v1,v2)


