## **A.Convolutional horses and humans**

### **1. Describe the ImageDataGenerator() command and its associated argument.  What objects and arguments do you need to specify in order to flow from the directory to the generated object?  What is the significance of specifying the target_size = as it relates to your source images of varying sizes? What considerations might you reference when programming the class mode = argument?  How difference exists when applying the ImageDataGenerator() and .flow_from_directory() commands to the training and test datasets?**

### **2. Describe the model architecture of the horses and humans CNN as you have specified it.  Did you modify the number of filters in your Conv2D layers?  How do image sizes decrease as they are passed from each of your Conv2D layers to your MaxPooling2D layer and on to the next iteration?  Finally, which activation function have you selected for your output layer?  What is the significance of this argument’s function within the context of your CNN’s prediction of whether an image is a horse or a human?  What functions have you used in the arguments of your model compiler?**

## **B.Regression**

### **1.Using the auto-mpg dataset (auto-mpg.data), upload the image where you used the seaborn library to pairwise plot the four variables specified in your model.  Describe how you could use this plot to investigate the co-relationship amongst each of your variables.  Are you able to identify interactions amongst variables with this plot?  What does the diagonal access represent?  Explain what this function is describing with regarding to each of the variables.**

### **2.After running model.fit() on the auto-mpg.data data object, you returned the hist.tail() from the dataset where the training loss, MAE & MSE were recorded as well as those same variables for the validating dataset.  What interpretation can you offer when considering these last 5 observations from the model output?  Does the model continue to improve even during each of these last 5 steps?  Can you include a plot to illustrate your answer?  Stretch goal: include and describe the final plot that illustrates the trend of true values to predicted values as overlayed upon the histogram of prediction error.  **

## **C.Overfit and underfit**

### **1.What was the significance of comparing the 4 different sized models (tiny, small, medium, large)?  Can you include a plot to illustrate your answer?**
