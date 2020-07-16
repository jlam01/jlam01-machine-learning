### **1. What is TF Hub? How did you use it when creating your script for "text classification of movie reviews"?**

TensorFlow Hub is a library and platform for transfer learning. It was used for the first layer to embed the sentences in the model in the script for "text classification of movie reviews".

### **2. What are the optimizer and loss functions? How good was your "text classification of movie reviews" model?**

Optimizer and loss functions work together to help the model learn the relationships of the data and calculate how good or bad an answer is, tweaking until it makes the predictions as accurate as possible. 

### **3. In "text classification with preprocessed text" you produced a graph of training and validation lss. Add the graph to this response and provide a brief explanation.**

![image](https://user-images.githubusercontent.com/67992204/87699977-a14ba380-c763-11ea-92d5-80d8935f5376.png)

The dots in the graph represent the training loss with the line representing the validation loss. At each epoch, the training loss decreases. The validation loss levels outs as the amount of epochs increases, which shows overfitting.

### **4. Likewise do the same for the training and validation accuracy graph.**

![image](https://user-images.githubusercontent.com/67992204/87700214-f982a580-c763-11ea-82b0-0a93fab0fb75.png)

In this graph, the dots represent the training accuracy with the line representing the validation accuracy. At each epoch, the training accuracy increases. The validation accuracy peaks, which shows the overfitting of the model.

## **Error working with the code:**

Even after copying and pasting the code from tensorflow onto pycharm, I kept on getting errors with imdb_reviews so I haven't been able to complete the exercise on pycharm due to this:

![imdb_reviews_error](https://user-images.githubusercontent.com/67992204/87238143-e458f000-c3cc-11ea-9a38-faa51b2db325.png)

As a result, this exercise was done through google colab.
