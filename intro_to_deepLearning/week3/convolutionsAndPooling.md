## Question 1: Choose correct statements about convolutional layer:
* **Convolutional layer is a special case of a fully-connected layer**
* Convolutional layer provides translation invariance
* **Convolutional layer works the same way for every input patch**
* Convolutional layer doesn't need a bias term

## Question 2: Choose correct statements about pooling layer:
* Pooling layer reduces the number of convolutional filters
* **Pooling layer can reduce spatial dimensions (width and height of the 
input volume)**
* **Pooling layer provides translation invariance**
* Pooling layer is strictly differentiable

## Question 3: Back-propagation for convolutional layer first calculates 
the gradients as if the kernel parameters were not shared and then...
* Takes a maximum gradient for each shared parameter
* **Takes a sum of gradients for each shared parameter**
* Takes a mean of the gradients for each shared parameter
* Takes a minimum gradient for each shared parameter

## Question 4: Suppose you have a 10x10x3 colour image input and you 
want to stack two convolutional layers with kernel size 3x3 with 10 and 
20 filters respectively. How many parameters do you have to train for 
these two layers? Don't forget bias terms!

2100 *(3 * 3 * 3 + 1) * 10 + (3 * 3 * 10 + 1) * 20*

## Question 5: What receptive field do we have after stacking nn 
convolutional layers with kernel size k \times kk×k and stride 1? 
Layers numeration starts with 1. The resulting receptive field will be a 
square, input its side as an answer.

(k-1)*(n-1)+k
