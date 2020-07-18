### **A. Last week you did an exercise where you manually applied a 3x3 array as a filter to an image of two people ascending an outdoor staircase.  Modify the existing filter and if needed the associated weight in order to apply your new filters to the image 3 times.  Plot each result, upload them to your response, and describe how each filter transformed the existing image as it convolved through the original array and reduced the object size.  What are you functionally accomplishing as you apply the filter to your original array (see the following snippet for reference)?  Why is the application of a convolving filter to an image useful for computer vision?  Stretch goal: instead of using the misc.ascent() image from scipy, can you apply three filters and weights to your own selected image?  Again describe the results.**

**Filter 1 (-1, 2, -1, 0, 0, 0, 1, 2, 1):**

![image](https://user-images.githubusercontent.com/67992204/87746449-9c680d80-c7be-11ea-8620-b33c161d7afe.png)

This filter emphasized the horizontal lines in the image which would aid in identifying the handrails of the stairs.

**Filter 2 (-1, 0, 1, -2, 0, 2, -1, 0, 1):**

![image](https://user-images.githubusercontent.com/67992204/87746109-c5d46980-c7bd-11ea-8376-e6abe098f217.png)

This filter identified the vertical lines in the image such as the rungs of the stairs.

**Filter 3 (-1, -2, -1, -2, 0, 2, -1, 0, 1):**

![image](https://user-images.githubusercontent.com/67992204/87747243-b571be00-c7c0-11ea-8707-65c3625e4080.png)

This filter also emphasizes the rungs of the stairs and the support structures.

When you apply a filter to the image, you can extract raw features of an images while retaining the original image. The application of a convolving filter to an image helps aid in processing images. By extracting the raw features of an image through filtering, it helps the machine identify patterns and recognize key features, essential to identifying items.

### **B. Another useful method is pooling.  Apply a 2x2 filter to one of your convolved images, and plot the result.  In effect what have you accomplished by applying this filter?  Can you determine from the code which type of pooling filter is applied, and the method for selecting a pixel value (see the following snippet)?  Did the result increase in size or decrease?  Why would this method be useful?  Stretch goal:  again, instead of using misc.ascent(), apply the pooling filter to one of your transformed images.**

![image](https://user-images.githubusercontent.com/67992204/87748593-501fcc00-c7c4-11ea-98bf-7f2715f5939a.png)

Above is the pooled image of *filter 1* from question A. The size of the image significantly decreased by 1/4 of the original size, however the original extracted features were maintained and emphasized even further. This is due to the fact that this processing of pooling selects the pixels of the highest values in order to create the new image, reducing the amount of noise and the size of the image.

### **C. The lecture for today (Coding with Convolutional Neural Network) compared the application of our previously specified deep neural network with a newly specified convolutional neural network.  Instead of using the fashion_MNIST dataset, use the mnist dataset (the hand written letters) to train and compare your DNN and CNN output. Were you able to improve your model by adding the Conv2D and MaxPooling2D layers to your neural network?  Plot the convolutions graphically, include them in your response and describe them.  Edit the convolutions be changing the 32s to either 16 or 64 and describe what impact this had on accuracy and training time.  What happens if you add more convolution layers?**

After 8 epochs of training, the neural network was able to improve and reach the accuracy of 99.8%. The test accuracy is 0.9889000058174133.

