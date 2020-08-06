![image](https://user-images.githubusercontent.com/67992204/89578329-f416f900-d7ff-11ea-9ad5-17c821326183.png)

### **Problem Statement:**

When it comes to x-ray images, medical professionals, specifically radiologists, need to classify and identify problems within these images in order to help diagnose individuals. Through the classification of X-ray images using machine learning it can help medical professionals identify these issues at a much more efficient rate, allowing individuals to be diagnosed efficiently and effectively.

How can x-ray images be analyzed and categorized in way that is as accurate as possible to allow proper diagnoses of patients through machine learning?

In order to approach this issue, a model using a convolutional network (CNN) was chosen to categorize and analyze x-ray scans. As there are many types of x-ray scans, the model used will be analyzing pneumonic and normal lungs and identify the respective lung conditions.

While applying this model, an obstacle that may occur is through the accuracy of the scan performed, if any scans are unclear, the model may not be able to properly analyze the image. In addition, the model may vary in accuracy with the type of scan used.

### **Data:**

The data used here were chest x-ray images (anterior-posterior) of pneumonic and normal lungs from pediatric patients of 1-5 yrs old from Guangzhou Women and Children’s Medical Center, Guanzhou. The dataset contained a total of 5856 images used for training and testing.

https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia/download
