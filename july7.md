### **1. In Laurence Maroney’s video, What is ML, he compares traditional programming with machine learning and argues that the main difference between the two is a reorientation of the rules, data and answers.  According to Maroney, what is the difference between traditional programming and machine learning?**

According to Maroney, the traditional programing is when it is us humans taking in rules and data and answers coming out. Traditional programming involves the programmmers manually figuring out the rules for the answers we get. Meanwhile, machine learning involves inputting the answers into a machine and having it figure out the rules for the programmer.

### **2. With the first basic script that Maroney used to predict a value output from the model he estimated (he initially started with 10 that predicted ~31.  Modify the predict function to produce the output for the value 7.  Do this twice and provide both answers.  Are they the same?  Are they different?  Why is this so?**

22.000578 and 22.001621 are the answers I got. These are different answers because the model is recompiled and relearning the data set and there was no random seed set. If that was set, the answers would be the same.

### **3. Using the script you produced to predict housing price, take the provided six houses and train a neural net model that estimates the relationship between them.  Based on this model, which of the six homes present a good deal?  Which one is the worst deal?  Justify your answer.**

Based on my model, Hudgins presents the best deal as you would be spending $137,358 less than what the model predicted. Meanwhile, Church would present the worst deal as you would be paying $99,121 more than the model predicted. 

Ranking | House | # of Bedrooms | Price | Predicted Price | Difference
:---: | :--- | :---: | :---: | :---: | :---:
1 | Hudgins | 3 | $97,000 | $234,358 | `- $137,358`
2 | Mathews | 5 | $347,500 | $365,397 | - $17,897
3 | Mobjack | 4 | $289,000 | $299,878 | - $10,878
4 | New Point Comfort | 3 | $229,000 | $234,358 | - $5,358
5 | Moon | 2 | $250,000 | $168,839 | + $81,161
6 | Church | 4 | $399,000 | $299,878 | + $99,121
