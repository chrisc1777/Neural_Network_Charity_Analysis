# Neural_Network_Charity_Analysis
## Overview
Alphabet Soup is a non-profit foundation that dedicates funding to life-saving technologies. The president of the company has requested a machine-learning model that could predict which foundations are safe to donate to and which ones to avoid for risks of corruption. 

For this project, I utilized a neural network machine-learning model using the scikit-learn and Tensorflow library in Jupyter Notebook. With the "Charity" dataset I was able to preprocess the applications of 34,000 fundraising foundations. Once preprocessed, that data was compiled, trained, and evaluated for accuracy in the predicting model. 

## Results
•	Data Preprocessing
o	The chosen target for the model was the "IS_SUCCESSFUL" variable.
![ann1](https://user-images.githubusercontent.com/106359564/228892641-860d157a-6100-49e4-b156-2e914d5c8c86.png)

o	The variables chosen as features for the model were: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT".


o	The "EIN" and "NAME" columns were removed from the features of this model.




•	Compiling, Training, and Evaluating the Model
o	There were two hidden layers chosen for the model. The first layer had 80 neurons and the second had 40. The activation functions chosen for both input layers were ReLU. Since the predicting model is nonlinear, the ReLu is a reliable activation function for this scenario. The Sigmoid activation function was chosen for the output for its capability of prediction target.




o	My original model was only able to receive an accuracy score of 72.5%. After making changes for my second attempt, I was able to achieve a target performance of over 75%. The final accuracy score of the model was 78%.

![ann4](https://user-images.githubusercontent.com/106359564/228893530-412aed84-71f4-45e6-ad90-b955326c7c05.png)


o	To improve the performance I dropped one less column "NAME" from the original model which dropped two columns that included "EIN and "NAME". I also decreased the number of values for "NAME" and "ASK_AMT". Lastly, I used three ReLu activation hidden layers. The first layer had 90 neurons, the second had 40, and the third had 10.

![ann2](https://user-images.githubusercontent.com/106359564/228892699-13cc4022-b55f-4278-aed7-87e74362da86.png)
![ann5](https://user-images.githubusercontent.com/106359564/228893846-6fded30a-85ec-4867-b32f-eb4c7ef59a22.png)
![ann6](https://user-images.githubusercontent.com/106359564/228893862-a0ec1357-e3f2-44d8-a5e0-0c0885acea26.png)
![ann3](https://user-images.githubusercontent.com/106359564/228893387-4a456d49-5d55-4f7d-a400-f0ef9c03959c.png)


## Summary
After testing out my machine-learning model with different configurations I was able to achieve a higher accuracy score by dropping less features, removing many unique values for 2 additional bins, and adding three hidden layers. Since this neural network required a long data preparation process, I would recommend using the Random Forest Classifier model to receive similar and faster accuracy results but with much less code.




