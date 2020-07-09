**(1)In Laurence Maroney’s video, What is ML, he compares traditional programming with machine learning and argues that the main difference between the two is a reorientation of the rules, data and answers.  According to Maroney, what is the difference between traditional programming and machine learning?**

According to Maroney, the traditional programing is when it is us humans taking in rules and data and answers coming out. Traditional programming involves the programmmers manually figuring out the rules for the answers we get. Meanwhile, machine learning involves inputting the answers into a machine and having it figure out the rules for the programmer.

**(2)With the first basic script that Maroney used to predict a value output from the model he estimated (he initially started with 10 that predicted ~31.  Modify the predict function to produce the output for the value 7.  Do this twice and provide both answers.  Are they the same?  Are they different?  Why is this so?**


import tensorflow as tf
import numpy as np
from tensorflow import keras
model = tf.keras.Sequential([keras.layers.Dense(units=1, input_shape=[1])])
model.compile(optimizer='sgd', loss='mean_squared_error')
xs = np.array([-1.0, 0.0, 1.0, 2.0, 3.0, 4.0], dtype=float)
ys = np.array([-2.0, 1.0, 4.0, 7.0, 10.0, 13.0], dtype=float)
model.fit(xs, ys, epochs=500)
print(model.predict([7.0]))

[[22.000578]] and [[22.001621]] are the answers. These are different answers because the model is recompiled and relearning the data set and there was no random seed set. If that was set, the answers would be the same.

**(3)Using the script you produced to predict housing price, take the provided six houses and train a neural net model that estimates the relationship between them.  Based on this model, which of the six homes present a good deal?  Which one is the worst deal?  Justify your answer.**

