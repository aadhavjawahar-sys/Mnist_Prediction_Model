# Mnist_Prediction_Model

A popular machine learning model that many elementary data scientists enjoy testing out is one that employs the MNIST dataset. This experiment involves using a 28x28 pixel image of black and white pixels, and the *Neural Network** predicts which number (0-9) has been drawn.

> My Neural Network model was trained using 600 sets of images, some with slight rotations to account for irregularities in human drawing.

***

## Data Processing

The *MNIST* dataset is a publicly available file which can be found on [Kaggle](https://www.kaggle.com/datasets/hojjatk/mnist-dataset). It consists of a sample of 600 pixelated numerical images split into a 2-dimension array for each of the pixels of the 28x28 image. The Neural Network was trained using a convolutional neural network where the final layer used a SoftMax activation function for selecting the digits category from 0-9. 

The model was trained using the **adam** optimizer (adaptive moment estimation). Its cost function used **sparse categorical cross entropy**, which outputted the respective probabilities for each category. This was used to give the top 3 chosen categories (numbers) for each given image.

***

## Model Accuracy

The model has a generally high accuracy of 98%+ for both training and testing data.


