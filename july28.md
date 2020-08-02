## **Word Embeddings**

### **1. Why is using one-hot encoding an inefficient towards vectorizing a corpus of words?  How are word embeddings different? (see this video https://www.youtube.com/watch?v=EEk6OiOOT2c )**

The use of one-hot encoding is inefficient towards vectoring a corpus of words as it involves the input of the number of words in rows and columns. Word embedding not only does the same as one-hot encoding but it can also get trained to understand the meanings of certain words through a model.

### **2. Compile and train the model from the tensorflow exercise.  Plot the training and validation loss as well as accuracy.  Post your plots and describe them.**

![image](https://user-images.githubusercontent.com/67992204/89113713-71c6b780-d442-11ea-9213-a2b2b414f6d8.png)

The above graph represents the training and validation loss over a certain number of epochs with the dots representing the training loss and line representing the validation loss. After 2 epochs, the graph represents the model being overfit by the increasing validation loss.

![image](https://user-images.githubusercontent.com/67992204/89113720-81460080-d442-11ea-8647-0a6a9ecce8c1.png)

The above graph here represents the training and validation accuracy over a certain number of epochs with the dots representing the training accuracy and the line representing the validation accuracy. According to the graph, approximately the 6th epoch is the best place to stop the model training as it seems to be overfit after.

## Text Classification with an RNN

### **1. Again compile and train the model from the tensorflow exercise.  Plot the training and validation loss as well as accuracy.  Stack two or more LSTM layers in your model.  Post your plots and describe them**
