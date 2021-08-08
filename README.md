# MNIST (Modified-National-Institute-of-Standards-and-Technology) Image Classification model

Aim: To build a supervised neural network that can distinguish between handwritten digits numbered 0-9. The model is trained on images taken from the MNIST database that consists of 70,000 images, 60,000 images in training data & 10,000 images in testing data.

Example of MNIST images -

![image](https://user-images.githubusercontent.com/59203913/128639453-e8774f27-b9c8-4fe8-8124-c49a122c0c98.png)

Result: The model has shown a prediction accuracy of ~98%.

Libraries used: Tensorflow, Matplotlib, Numpy

Development Environment: Google Colab.


MNIST dataset - It is a dataset consisting of 70,000 small square 28×28 pixel grayscale images of handwritten single digits between 0 and 9. Each pixel is associated with a number ranging from 0 to 255 which denotes the intensity of the pixel's color. 0 is taken as black & 255 is taken as white. 
The original dataset has black & white images. The images displayed in our project are colored as the imshow() method of matplotlib has been used.

The MNIST database is available at http://yann.lecun.com/exdb/mnist/
