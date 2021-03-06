# Reducing-Commercial-Aviation-Fatalities
### I wrote a detailed blog on my approach to this problem on medium, I would recommend you to read it for better understanding of the problem:

### Link- https://atharvamusale.medium.com/reducing-commercial-aviation-fatalities-c335757e8d01

# Objective-
Source: https://www.kaggle.com/c/reducing-commercial-aviation-fatalities. Most of the flight related fatalities stems from loss of " Aeroplane State Awareness". That is, ineffective attention management on the part of pilots who may be distracted, sleepy or in other dangerous cognitive states. In this competition, kagglers are asked to build a model for predicting the pilot's state of awareness based on the data consisting of some information like ECG, EEG, GSR(Galvanic Skin Response), Respiration etc. The model built using this data will be used to detect if pilot is going into troubling physical condition or not. So that, using the result of this model pilots can be alerted and the accidents in aviation industry can be reduced.

# Mapping into ML problem - 
Based on the data given like ECG,EEG,GSR and othe features we are supposed to predict the state of awareness of pilot. There are four classes as an output:
1. Baseline 
2. Channelized Attention (CA) - This type of attention is focussed on one task and no other tasks were attended by the pilot during this stage.
3. Diverted Attention(DA) - This type of attention is diverted by the processes related to the decision making.(Can be thought as multitasking, as attention is given to various tasks).
4. Startle/Surprise(SS) - Involves surprise or sudden change in scenario when attention level gets disrupted.

# Evaluation Metric- 
The metric whcih is used is Multi Class Log-Loss. 
![ScreenShot](https://github.com/AtharvaMusale/Reducing-Commercial-Aviation-Fatalities/blob/master/Screenshot%202021-01-26%20at%208.15.06%20AM.png)

# Algorithms Tried - 
1. Logistic Regression
2. Naive Bayes
3. Decision Trees
4. Random Forest
5. LightGBM

# Best Model and its result - 
LightGBM outperformed all the other algorithms and the results I got were as follows:
![ScreenShot](https://github.com/AtharvaMusale/Reducing-Commercial-Aviation-Fatalities/blob/master/Screenshot%202021-01-26%20at%208.22.02%20AM.png)

