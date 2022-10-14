1. This assignment will require Python 3.6 or above. 
2. Install the required Python package for deep learning:
    pip install -r requirements.txt

# Group
King

## Team Members
Rohan Anand
Jai Patel
Ishan Rathi
_________________________________________________________________________________
# Written Report

## Description of Experiments performed

In order to achieve the highest validation accuracy, many hyperparameters and activation functions were tested.

Hyperparameters:

We tested both adam and sgd optimizers

We tested epochs of all sizes including 10, 50, 100, 250, 500

We tested hidden sizes of 64, 128, 156, 256

We tested scaling factors of 255

Activation Functions:

We tested relu, selu, tanh, and sigmoid

We tested these activation functions as layers in different orders, building the network in a variety of ways

Some accuracies  we found were as followed:

Epoch: 10
Hidden: 64
Acc: 34.09

Epoch: 50
Hidden: 128
Acc: 39.12

Epoch: 100
Hiden: 64
Acc: 39.26


## For best performing model

### Description of Model and Model Training Procedure

The best performing model had the following hyper-parameters:

Optimizer - adam

Epochs - 100

Hidden Size - 128

Scaling Factor - 255

The best performing model had the following hidden layers:

First layer - activation function relu

Second layer - activation function relu

Third layer - activation function sigmoid


The model was run many times, resulting in an approximate accuracy of 40% each time indicating our best performing model

### Training and Validation Performance Plot

![alt text](https://github.com/ishan190425/Project3RCSMD/blob/main/AccuracyPlot.jpeg?raw=true)

### Performance (Accuracy, Precision, and Recall) of Best Performing Model

The performance of our best performing model:

Accuracy - 0.4108999967575073

Precision - 0.4109

Recall - 0.4109

### Confusion Matrix of Best Performing Model

Confusion Matrix
 [[362  81  81  48  81  39  57  68 132  51]
 [ 36 547   4  42  14  16  33  37  96 175]
 [ 81  31 273 151  98 131 106  71  41  17]
 [ 27  52  53 325  52 166 149  78  47  51]
 [ 75  34  95 114 223  92 143 139  53  32]
 [ 31  20  80 222  37 369  90  90  31  30]
 [ 32  50  52 147  62  70 479  38  39  31]
 [ 38  27  45  93  48  90  52 532  36  39]
 [ 87  93  17  64  35  27  39  35 550  53]
 [ 43 212  19  62  11  21  40  61  82 449]]

![alt text](https://github.com/ishan190425/Project3RCSMD/blob/main/ConfusionMatrix.jpeg?raw=true)

### Visualization of three misclassified images

Image 1:


![alt text](https://github.com/ishan190425/Project3RCSMD/blob/main/Misclassified1.jpeg?raw=true)

image 2:


![alt text](https://github.com/ishan190425/Project3RCSMD/blob/main/Misclassified2.jpeg?raw=true)

Image 3:


![alt text](https://github.com/ishan190425/Project3RCSMD/blob/main/Misclassified3.jpeg?raw=true)


Some reasons why the images could have been misclassified is the images could be very simiar to another where the pixel differences could not be identified by the hidden layers used. 
This maybe due to the lack of depth and complexity of the hidden layers.
