# Handwritten Digit Recognition

## Project Overview
The project is to identify handwritten digits (0-9) from image with Convolutional Neural Network (CNN). It is a part of the CodeAlpha Machine Learning internship, #3.

## Dataset
MNIST dataset (preloaded by Keras): 60,000 training images and 10,000 test images. The images are grayscale, with dimensions: 28 x 28. The distribution of the 10 classes (digits 0 to 9) is fairly even.

## Approach
1. Interpreted and analysed the data.
2. Scaled pixel values from 0-255 to 0-1 and reshaped images to (28, 28, 1).
3d. Developed a CNN comprising of two convolution + max pooling blocks, a dense layer and a softmax output layer.
5. Tried training the model for 5 epochs using Adam, with a validation set of 10% of its training data.
Evaluated accuracy, confusion matrix, classification report and training curves of the model.

## Results
- Training accuracy: 99.04%
- Validation accuracy: 99.03%
- Test accuracy: 98.93% (107 wrong predictions out of 10,000 images)
The precision, recall and F1-score are all between 0.98 and 0.99 for each digit.

The training curve and validation curve are not significantly different, indicating that the model is not overfitting.

## Limitation
The most often wrong answer is "2" for 7 and "9" for 4. Most of the images that are incorrectly predicted are written in an unusual manner. This is a digit recognition project. Can be expanded to letters (EMNIST) or extended to full words with sequence models like CRNN.

## Tools Used
Python, TensorFlow/Keras, NumPy, matplotlib, scikit-learn, Google Colab

## How to Run
Open the notebook in Google Colab or Jupyter and run all cells from top to bottom.
