## **A.Convolutional horses and humans**

### **1. Describe the ImageDataGenerator() command and its associated argument.  What objects and arguments do you need to specify in order to flow from the directory to the generated object?  What is the significance of specifying the target_size = as it relates to your source images of varying sizes? What considerations might you reference when programming the class mode = argument?  How difference exists when applying the ImageDataGenerator() and .flow_from_directory() commands to the training and test datasets?**

ImageDataGenerator() from the Keras library takes images and transforms them. The generator is then created by flowing them out of the directory to the generated object by calling the flow from the directory method. The size of the images are required to be specified and the images used should be rescaled and resized. In addition, the batch size can be specified. Specifying the target size is important as varying the sizes of the images may mess up while being inputted into the model. When programming the class mode argument, you should reference to the amount of classes you have. If you have 2 classes, keep it at binary; if you have more than 2 classes, the class mode should be categorical.

### **2. Describe the model architecture of the horses and humans CNN as you have specified it.  Did you modify the number of filters in your Conv2D layers?  How do image sizes decrease as they are passed from each of your Conv2D layers to your MaxPooling2D layer and on to the next iteration?  Finally, which activation function have you selected for your output layer?  What is the significance of this argument’s function within the context of your CNN’s prediction of whether an image is a horse or a human?  What functions have you used in the arguments of your model compiler?**

The model contains 3 Conv2d layers, each followed by a maxpool layer. Next, there is a flatten followed by two dense layers. As you proceed through each convolution and maxpool pair, the size of the images reduces. Sigmid activation was selected for the binary classifier. This allows you to have only one neuron and have an output of 0 for one class and 1 for the other class. For the model compiler, the loss function called binary cross entropy and an optimizer called RMS prop were used.

## **B.Regression**

### **1.Using the auto-mpg dataset (auto-mpg.data), upload the image where you used the seaborn library to pairwise plot the four variables specified in your model.  Describe how you could use this plot to investigate the co-relationship amongst each of your variables.  Are you able to identify interactions amongst variables with this plot?  What does the diagonal access represent?  Explain what this function is describing with regarding to each of the variables.**

![image](https://user-images.githubusercontent.com/67992204/87864569-d1e43680-c937-11ea-9a30-9a8ca99ca479.png)

This plot is used to investigate the co-relationship amongst the variables, in this case the 4 variables: MSG, Cylinders, Displacement, and Weights. Using the plots, u can visualize the trends between each variable. For example, as the displacement of the car increases, number of weights also increase. Kernel density is used to determine the univariable plots at the diagonals.

### **2.After running model.fit() on the auto-mpg.data data object, you returned the hist.tail() from the dataset where the training loss, MAE & MSE were recorded as well as those same variables for the validating dataset.  What interpretation can you offer when considering these last 5 observations from the model output?  Does the model continue to improve even during each of these last 5 steps?  Can you include a plot to illustrate your answer?  Stretch goal: include and describe the final plot that illustrates the trend of true values to predicted values as overlayed upon the histogram of prediction error.**

![image](https://user-images.githubusercontent.com/67992204/87864867-b67b2a80-c93b-11ea-93bf-0fc75131d629.png)

Using this plot, you can infer that the model can no longer improve after the last 5 epochs as the graph has leveled out. Increasing the number of epochs will not aid in improving the accuracy of the model.

## **C.Overfit and underfit**

### **1.What was the significance of comparing the 4 different sized models (tiny, small, medium, large)?  Can you include a plot to illustrate your answer?**

![image](https://user-images.githubusercontent.com/67992204/87867970-db819480-c95f-11ea-99e7-96d92dea4294.png)

As seen through this graph, as the models got larger in size, they became high overfit as the number of epochs increase. In addition, they increasingly took much longer to process.
