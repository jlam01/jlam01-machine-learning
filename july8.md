**A. In the video, First steps in computer vision, Laurence Maroney introduces us to the Fashion MNIST data set and using it to train a neural network in order to teach a computer “how to see.”  One of the first steps towards this goal is splitting the data into two groups, a set of training images and training labels and then also a set of test images and test labels.  Why is this done?  What is the purpose of splitting the data into a training set and a test set?**

The data is split into training and test groups in order to train the model and neural networks to understand the relationships between the data. Through that, the neural network can predict answers through the test group. In order to test how well the model does through the training, we use test data that the model has not come across. Since it has not come across the test data, it is not the machine just memorizing the training data and rather understands the relationship between the data itself.

**B. The fashion MNIST example has increased the number of layers in our neural network from 1 in the past example, now to 3.  The last two are .Dense layers that have activation arguments using the relu and softmax functions.  What is the purpose of each of these functions.  Also, why are there 10 neurons in the third and last layer in the neural network.**

Relu function determines that if an outpt of a neuron is less than 0 it will be set to zero, ensuring that negative results do not skew the results. Softmax functions, on the other hand, aids in finding the most likely candidate out of the selection of choces. This is most commonly seen on the last layer of the neural network.

In the fashion MIST example, there are 10 neurons as there were 10 possible categories for the images to be sorted into. If there were more or less categories, the number of neurons would be adjusted more or less to the same amount of categories to be sorted into.

**C. In the past example we used the optimizer and loss function, while in this one we are using the function adam in the optimizer argument and sparse_categorical-crossentropy for the loss argument.  How do the optimizer and loss functions operate to produce model parameters (estimates) within the model.compile() function?**

**D. Using the mnist drawings dataset (the dataset with the hand written numbers with corresponding labels) answer the following questions.**

***1. What is the shape of the images training set (how many and the dimension of each)?***

***2. What is the length of the labels training set?***

***3. What is the shape of the images test set?

***4. Estimate a probability model and apply it to the test set in order to produce the array of probabilities that a randomly selected image is each of the possible numeric outcomes (look towards the end of the basic image classification exercises for how to do this — you can apply the same method applied to the Fashion MNIST dataset but now apply it to the hand written letters MNIST dataset).***

5. Use np.argmax() with your predictions object to return the numeral with the highest probability from the test labels dataset.

6. Produce the following plot for your randomly selected image from the test dataset
