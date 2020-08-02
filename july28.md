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

![image](https://user-images.githubusercontent.com/67992204/89114412-08e33d80-d44a-11ea-84da-0d8f0a9ca62b.png)

The above graph here is the training and validation accuracy over a certain number of epochs with the training accuracy being blue and the validation accuracy being orange. After 1 epoch, the validation accuracy reduces below the training accuracy and plateaus.

![image](https://user-images.githubusercontent.com/67992204/89114417-113b7880-d44a-11ea-9cd1-9f157f25cc3a.png)

The above graph represents the training and validation loss over a certain number of epochs with the training loss being blue and the validation loss represented by the orange. After 1 epoch, the training loss reduces significantly, showing that the model has gotten overfit.

![image](https://user-images.githubusercontent.com/67992204/89114420-1ac4e080-d44a-11ea-9b22-1268f1a2131d.png)

The above graph here represents the training and validation accuracy over a certain number of epochs on a model with 2 or more LSTM layers. The training accuracy is blue with the validation accuracy being orange. After 1 epoch, the validation accuracy goes below the training accuracy and plateaus, representing the overfitting of the model.

![image](https://user-images.githubusercontent.com/67992204/89114422-21535800-d44a-11ea-9766-907718de310f.png)

The above graph here shows the training and validation loss over a certain number of epochs on a model with 2 or more LSTM layers. The training loss  is shown in blue with the validation loss represented by the orange. After 1 epoch, the training loss reduces significantly, showing that the model has gotten overfit.

