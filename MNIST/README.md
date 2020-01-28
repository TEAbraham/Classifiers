# Image Classification

## 1. Download the MNIST Data

The MNIST database contains 60,000 training images and 10,000 testing images taken from American Census Bureau employees and American high school students.

## 2. Reshape and Normalize the Images

To be able to use the dataset in Keras API, we need 4-dims numpy arrays. However, as we see above, our array is 3-dims. In addition, we must normalize our data as it is always required in neural network models. We can achieve this by dividing the RGB codes to 255 (which is the maximum RGB code minus the minimum RGB code). 

## 3. Build the Convolutional Neural Network

We will build our model by using high level Keras API which uses either TensorFlow or Theano on the backend. I would like to mention that there are several high level TensorFlow APIs such as Layers, Keras, and Estimators which helps us create neural networks with high level knowledge. However, this may lead to confusion since they all varies in their implementation structure. Therefore, if you see completely different codes for the same neural network although they all use tensorflow, this is why. I will use the most straightforward API which is Keras. Therefore, I will import the Sequential Model from Keras and add Conv2D, MaxPooling, Flatten, Dropout, and Dense layers.

## 4. Compile and Fit the Model

Now it is time to set an optimizer with a given loss function which uses a metric. Then, we can fit the model by using our train data.

## 5. Evaluate the Model

Finally, you may evaluate the trained model with x_test and y_test.