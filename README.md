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

![Crazy Accuracy Trust](https://github.com/aadhavjawahar-sys/Mnist_Prediction_Model/blob/main/images/accuracy_Mnist.png)

***

## Working Model Demonstration

To interact with my model, I built a graphical user interface with the [gradio](https://gradio.app/) python  module. Initialy, the user sees a box to draw their pixelated number, where you can change the stroke thickness using one of the sidebar options.

![Crazy Accuracy Trust](https://github.com/aadhavjawahar-sys/Mnist_Prediction_Model/blob/main/images/demonstration1_Mnist.png)

Once you complete your drawing, you can press the Calculate Prediction button to see the output.

![Crazy Accuracy Trust](https://github.com/aadhavjawahar-sys/Mnist_Prediction_Model/blob/main/images/demonstration2_Mnist.png)

The processed 28x28 pixel output is shown in one box at its real size.

![Crazy Accuracy Trust](https://github.com/aadhavjawahar-sys/Mnist_Prediction_Model/blob/main/images/demonstration3_Mnist.png)

Finally, the top prediction, along with the confidence level and next best 2 options are displayed.

***

## Future Direction

While the model is fairly decent at predicting the number if written in the same style as the training data, it's lacking when the style changes slightly or when images are rotated, making it too dependent on the training data. If I spend more time on the model, I will focus on expanding the dataset to include rotations and different styles, and train up to at least 5 epochs (Trained it with 2 epochs for given model) to improve accuracy. After adding this features in the future, the model will be much better at making its predictions. Thank you for viewing!


