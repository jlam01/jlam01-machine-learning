## **A. Write a Problem Statement.  Introduce your topic, quantify its significance, and describe the problem as a process.  Identify and quantify significant obstacles to solving your problem.  Demonstrate why your topic is important, and why the obstacles associated with your topic are significant both globally as well as within the context of your selected application. Describe and analyze the complex nature of the process you are investigating, including the system, the environment, agents and networks. Describe and analyze scope, scale and hierarchy of processes and sub-processes. Describe and analyze factors that contribute to quantified obstacles.  Describe and analyze process oriented causes-effect relationships.**

**Topic:**
Medical professionals, specifially radiologists need to classify and identify x-ray images in order to help diagnose individuals. 

**Significance:**
Through the classification of X-ray images using machine learning, it can help medical professionals identify individuals with problems shown through their x-ray scans much easier and quicker. This will help medical professionals diagnose individuals at a much quicker speed, which is important if the issue is something urgent.

**Description of the problem as a process**:
In order to diagnose a issue that can be found through x-ray scans, the medical professional must analyze and compare the x-ray images with a normal healthy x-ray image. This requires a lot of time and is crucial expecially if it is something time-limited. Having something that can classify the x-ray images will greatly reduce the amount of time required to analyze these x-ray images. 

**Obstacles:**
Firstly, we need to somehow obtain the x-ray images. In order to train the model, we must already have a set of images that are already classfied based on what is considered a normal healthy x-ray image and an unhealthy one. In addition, there may be several conditions shown in that x-ray scan and the model has to be able to identify which difference is the important thing to look out for in certain x-ray scans if we are trying to pinpoint certain illnesses rather than whether or not it is generally healthy.


## **B.Up next for your final project: data (then after that: methods)**
As there are many x-ray images and many cases to look into, I will be looking at pneumonia and x-ray images of the lungs between a healthy patient and a pnemonic patient.

## **C.Go to the website http://cs229.stanford.edu/proj2017/ and review some of the posters for the University of Stanford’s Fall 2017 machine learning course.  Consider how you will design and present your final project as a poster.**

## **D.Describe your implementation of the cats & dogs exercise.  How did you setup the data?**  

### **1.Which optimizer have you selected, and how might it compare to other possible choices?  (have a look at this site - https://towardsdatascience.com/understanding-rmsprop-faster-neural-network-learning-62e116fcf29a)**

The RMSprop, root mean square prop, optimizer was chosen over Rprop as it not only accounts for the big dataset that is used for cats and dogs but also for the gradients in the images used. RMSprop keeps the moving average of the squared gradients for each weight and divides the gradient by square root the mean square.

### **2.Describe your selected loss function and it’s implementation.  How is it effectively penalizing bad predictions? (have a look at this site - https://towardsdatascience.com/understanding-binary-cross-entropy-log-loss-a-visual-explanation-a3ac6025181a)**

The loss function selected is binary crossentropy due to the fact that it is a classification between only 2 things, thus binary. Binary crossentropy calcuates the probability of picking one out of the available 2 classifications, follows that with the calculation of entropy and crossentropy, and compares it in a Kullback-Leiber Divergence.

### **3.What is the purpose of the metric= argument in your model.compile() function? (look here - https://keras.io/api/metrics/)**

The metric argument calculates for how often the predicted answers are accurate to the actual answers.

### **4.Plot the accuracy and loss results for both the training and test datasets.  Include these in your response.  Assess the model and describe how good you think it performed.5.Use the model to predict 3 dog images and 3 cat images.  Upload you images and the prediction.  How did your model perform in practice?  Do you have any ideas of how to improve the model’s performance?**

**Accuracy:**

![image](https://user-images.githubusercontent.com/67992204/88450269-bf786a00-ce1b-11ea-8537-fad73de232fb.png)

This graph above represents the training and validation accuracy. Around
**Loss:**

![image](https://user-images.githubusercontent.com/67992204/88450277-ca32ff00-ce1b-11ea-914f-655d6d1a386a.png)

**Dogs and Cats:**
![image](https://user-images.githubusercontent.com/67992204/88450326-29910f00-ce1c-11ea-9340-8cf05cb4df22.png)
![image](https://user-images.githubusercontent.com/67992204/88450370-7a086c80-ce1c-11ea-8ba6-61506705f8bf.png)
![image](https://user-images.githubusercontent.com/67992204/88450386-91475a00-ce1c-11ea-9254-32ff3b6ed675.png)
![image](https://user-images.githubusercontent.com/67992204/88450400-a6bc8400-ce1c-11ea-8158-3f95ef75c43e.png)
![image](https://user-images.githubusercontent.com/67992204/88450421-c8b60680-ce1c-11ea-9473-352e80892bdc.png)
![image](https://user-images.githubusercontent.com/67992204/88450428-d4093200-ce1c-11ea-8646-d74c0ca5c3e0.png)

Out of the 

