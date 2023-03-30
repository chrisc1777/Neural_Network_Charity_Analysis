# Neural_Network_Charity_Analysis
## Overview
Alphabet Soup is a non-profit foundation that dedicates funding to life-saving technologies. The president of the company has requested a machine-learning model that could predict which foundations are safe to donate to and which ones to avoid for risks of corruption. 

For this project, I utilized a neural network machine-learning model using the scikit-learn and Tensorflow library in Jupyter Notebook. With the "Charity" dataset I was able to preprocess the applications of 34,000 fundraising foundations. Once preprocessed, that data was compiled, trained, and evaluated for accuracy in the predicting model. 

## Results
•	Data Preprocessing
o	The chosen target for the model was the "IS_SUCCESSFUL" variable.
![ann1](https://user-images.githubusercontent.com/106359564/228892641-860d157a-6100-49e4-b156-2e914d5c8c86.png)

o	The variables chosen as features for the model were: "NAME", "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT"

o	The "EIN" was removed from the features of this model

![ann2](https://user-images.githubusercontent.com/106359564/228892699-13cc4022-b55f-4278-aed7-87e74362da86.png)

•	Compiling, Training, and Evaluating the Model
o	There were three hidden layers chosen for the model. The first layer had 90 neurons, the second had 40, and the third had 10. The activation functions chosen for all three input layers were ReLU. Since the predicting model is nonlinear, the ReLu is a reliable activation function for this scenario. The Sigmoid activation function was chosen for the output for its capability of prediction target.

![ann3](https://user-images.githubusercontent.com/106359564/228893387-4a456d49-5d55-4f7d-a400-f0ef9c03959c.png)


o	I was able to achieve a target performance of over 75%. The final accuracy score of the model was 78%.

![ann4](https://user-images.githubusercontent.com/106359564/228893530-412aed84-71f4-45e6-ad90-b955326c7c05.png)

o	Steps taken to improve and increase model performance:

![ann5](https://user-images.githubusercontent.com/106359564/228893846-6fded30a-85ec-4867-b32f-eb4c7ef59a22.png)
![ann6](https://user-images.githubusercontent.com/106359564/228893862-a0ec1357-e3f2-44d8-a5e0-0c0885acea26.png)




