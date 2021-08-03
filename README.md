# MNIST-Modified-National-Institute-of-Standards-and-Technology-Image-Classification-model

Aim: To build a deep learning model that can distinguish between handwritten digits numbered 0-9. The dataset used consists of 70,000 images, 60,000 in train data & 10,000 in test data by default.


Steps:
1. Loaded the dataset
2. Extracted 10% of the training set for validation & converted the number of validation samples to int
3. Extracted test data  converted number of test samples to int
4. Scaled all the inputs/pixels of an image by dividing them by 255 & converted them to float (complete train_data). Each pixel has a greyscale value (color) ranging from 0-255, 0 being black & 255 being white. All the pixels now have a value between 0 & 1. The scaled variable was then mapped to the entire train dataset & test dataset. 
5. Data shuffling to prevent bias while learning- data shuffled 10,000 values at a time, shuffled train_data & validation_data extracted. 
6. Optimized the model using stochastic gradient descent instead of gradient descent as it processes large datasets faster. The batch size was chosen as 1000 for train, test, & validation sets.
7. Validation data was put in 2-tuple format (validation_train & validation_test)
8. Model outline - input_size=784(28*28), output_size=10, hidden_layer_size=500
9. Image flatted, 3 hidden layers created with Dense() which multiplies the inputs with their weights & adds biases. Activation function chosen=Relu. Relu chosen as it can classify better than other activation functions & doesn't pose the issue of vanishing gradient descent.
10. Output_layer specified with softmax activation function (Activation Function used in multi-classification models).
11. 'Adam Optimizer' chosen as it is the most efficient of all optimizers as it uses both learning rate & momentum.
12. Loss function chosen=sparse_categorical_crossentropy (as the outputs are one-hot encoded).
13. Training - Number of epochs chosen=5, data fit to the model.
14. Testing - Model tested for accuracy & loss.
15. Finally, model's learning tested with an MNIST image.  
