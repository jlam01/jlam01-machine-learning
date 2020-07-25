A. Boosted Trees

1. What is a one-hot-encoded column and why might it be needed when transforming a feature?  Are the source values continuous or discrete?

A one-hot-encoded column separates columns into categories. This is needed when transforming a feature as it helps identify specific features through the separation. The source values are discrete as we are working with categorical data rather than numerical data. Numerical data would classify as a continuous source value.

2. What is a dense feature?  For example, if you execute example = dict(dftrain) and then tf.keras.layers.DenseFeatures(your_features)(your_object).numpy(), how has the content of your data frame been transformed?  Why might this be useful?

A dense feature will define any lack of data as the value of 0. This is especially useful when a 0 features are important to predict within a model.

3. Provide a histogram of the probabilities for the logistic regression as well as your boosted tree model.  How do you interpret the two different models?  Are their predictions essentially the same or is there some area where they are noticeable different.  Plot the probability density function of the resulting probability predictions from the two models and use them to further illustrate your argument.  Include the ROC plot and interpret it with regard to the proportion of true to false positive rates, as well as the area under the ROC curve.  How does the measure of the AUC reflect upon the predictive power of your model?

B. Boosted Trees continued (with model understanding)

1. Upload your feature values contribution to predicted probability horizontal bar plot as well as your violin plot.  Interpret and discuss the two plots.  Which features appear to contribute the most to the predicted probability?

2.Upload at least 2 feature importance plots.  Which features are the most important in their contribution to your models predictive power?

3.Stretch goal: Modify the visualization formula.  Plot your output and provide an interpretation.  Which estimator was more effective at reproducing the probability model that was used to generate the instance of data that was synthetically generated?
