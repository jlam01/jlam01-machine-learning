**A. In the video, First steps in computer vision, Laurence Maroney introduces us to the Fashion MNIST data set and using it to train a neural network in order to teach a computer “how to see.”  One of the first steps towards this goal is splitting the data into two groups, a set of training images and training labels and then also a set of test images and test labels.  Why is this done?  What is the purpose of splitting the data into a training set and a test set?**

B.The fashion MNIST example has increased the number of layers in our neural network from 1 in the past example, now to 3.  The last two are .Dense layers that have activation arguments using the relu and softmax functions.  What is the purpose of each of these functions.  Also, why are there 10 neurons in the third and last layer in the neural network.

C.In the past example we used the optimizer and loss function, while in this one we are using the function adam in the optimizer argument and sparse_categorical-crossentropy for the loss argument.  How do the optimizer and loss functions operate to produce model parameters (estimates) within the model.compile() function?

D.Using the mnist drawings dataset (the dataset with the hand written numbers with corresponding labels) answer the following questions.

1.What is the shape of the images training set (how many and the dimension of each)?

2.What is the length of the labels training set?

3.What is the shape of the images test set?

4.Estimate a probability model and apply it to the test set in order to produce the array of probabilities that a randomly selected image is each of the possible numeric outcomes (look towards the end of the basic image classification exercises for how to do this — you can apply the same method applied to the Fashion MNIST dataset but now apply it to the hand written letters MNIST dataset).

5.Use np.argmax() with your predictions object to return the numeral with the highest probability from the test labels dataset.

6.Produce the following plot for your randomly selected image from the test dataset
