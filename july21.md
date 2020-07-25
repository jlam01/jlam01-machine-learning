## **A. Premade estimators**

### **1. How did you split the labels from the training set?  What was the name of the labels dataset?**

The labels were split from the training set through the use of pop to remove the labels of the dataset. The labels used were Setosa, Versicolor, and Virginica.

### **2. List 5 different estimators from tf.estimator and include the base command as you would write it in a script (for example this script used the tf.estimator.DNNClassifier() function from the API).**

DNNClassifier = tf.estimator.DNNClassifier()

DNNEstimator = tf.estimator.DNNEstimator()

DNNLinearCombinedClassifier = tf.estimator.DNNLinearCombinedClassifier()

DNNRegressor = tf.estimator.DNNRegressor()

DNNLinearCombinedRegressor = tf.estimator.DNNLinearCombinedRegressor()

### **3. What are the purposes input functions and defining feature columns?**

The input function returns a dataset containing a two-element tuple, converting the original dataset into smaller datasets. If training mode is set to true, the data can be shuffled around. The feature columns define what the input data is and how it is to be used.

### **4. Describe the command classifier.train() in detail.  What is the classifier and how did you define it?  Which nested function (and how have you defined it) are you applying to the training and test detests?**

The command classifier.train() runs the model with the provided data. Classifier is a DNNClassifier model containing 2 hidden layer: a 30 neuron layer and a 10 neuron layer. The model is given data in the small datasets from the input function 

### **5. Redefine your classifier using the DNNLinearCombinedClassifier() as well as the LinearClassifier().  Retrain your model and compare the results using the three different estimators you instantiated.  Rank the three estimators in terms of their performance.**

Rank | Classifier | Accuracy
--- | ---: | :---
1 | LinearClassifer | 0.967
2 | DNNClassifier | 0.767
3 | DNNLinearCombinedClassifier |  0.533

## **B. Build a Linear Model**

### **1. Using the dftrain dataset, upload an image where you used the seaborn library to produce a sns.pairplot().  Also include a histogram of age using the training set and compare it to the seaborn plot for that same feature (variable).  What interpretation can you provide of the data based on this plot?**

### **2. What is the difference between a categorial column and a dense feature?**

### **3. Describe the feature columns that have been input to your LinearClassifier().  How would you assess the result from your initial output?  What is the purpose of adding a cross featured column?  Did your attempt to capture the interaction between age and gender and incorporate it into your model improve performance?  Include and interpret your predicted probabilities and ROC curve plots.**
