![image](https://user-images.githubusercontent.com/67992204/89578329-f416f900-d7ff-11ea-9ad5-17c821326183.png)

### **Problem Statement:**

When it comes to x-ray images, medical professionals, specifically radiologists, need to classify and identify problems within these images in order to help diagnose individuals. Through the classification of X-ray images using machine learning it can help medical professionals identify these issues at a much more efficient rate, allowing individuals to be diagnosed efficiently and effectively.

How can x-ray images be analyzed and categorized in way that is as accurate as possible to allow proper diagnoses of patients through machine learning?

In order to approach this issue, a model using a convolutional network (CNN) was chosen to categorize and analyze x-ray scans. As there are many types of x-ray scans, the model used will be analyzing pneumonic and normal lungs and identify the respective lung conditions.

While applying this model, an obstacle that may occur is through the accuracy of the scan performed, if any scans are unclear, the model may not be able to properly analyze the image. In addition, the model may vary in accuracy with the type of scan used.

### **Data:**

The data used here were chest x-ray images (anterior-posterior) of pneumonic and normal lungs from pediatric patients of 1-5 yrs old from Guangzhou Women and Children’s Medical Center, Guanzhou. The dataset contained a total of 5856 images used for training and testing.

https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia/download

### **Method:**

![image](https://user-images.githubusercontent.com/67992204/89578470-2f192c80-d800-11ea-9098-a9c64179bc03.png)

The data was trained at 50 epochs with 100 steps per epoch.

### **Method Performance:**

After running the CNN model, the model was able to reach approximately 90% accuracy on the testing set and 97% accuracy on the training set; there was 0.3506 loss in the testing and  0.0772 loss in the training. This suggests the model is slightly overfit.


### **Project Proposal:**
As this project was performed on only chest x-ray scans, I would like to have been able to try out x-ray scans at other regions of the body as well as other scans such as MRI and CAT to see if machine learning is possible to be used in the field of radiology. I would need acquire these scans from radiologists with some already analyzed to be used for training. If possible, if the model works on any type of scan, then it would greatly help with the analysis of scans and help radiologists.
