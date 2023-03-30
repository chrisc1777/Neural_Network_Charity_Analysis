# Neural_Network_Charity_Analysis
## Overview
Alphabet Soup is a non-profit foundation that dedicates funding to life-saving technologies. The president of the company has requested a machine-learning model that could predict which foundations are safe to donate to and which ones to avoid for risks of corruption. 

For this project, I utilized a neural network machine-learning model using the scikit-learn and Tensorflow library in Jupyter Notebook. With the "Charity" dataset I was able to preprocess the applications of 34,000 fundraising foundations. Once preprocessed, that data was compiled, trained, and evaluated for accuracy in the predicting model. 

## Results
•	Data Preprocessing
o	The chosen target for the model was the "IS_SUCCESSFUL" variable.

<img width="532" alt="ann11" src="https://user-images.githubusercontent.com/106359564/228979529-40db0025-c014-44d2-b729-fc462b1392d2.png">



o	The variables chosen as features for the model were: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT".


o	The "EIN" and "NAME" columns were removed from the features of this model.

<img width="364" alt="ann7" src="https://user-images.githubusercontent.com/106359564/228977477-d982d80f-f412-445e-b43a-caaab8faf3d1.png">


•	Compiling, Training, and Evaluating the Model

o	There were two hidden layers chosen for the model. The first layer had 80 neurons and the second had 40. The activation functions chosen for both input layers were ReLU. Since the predicting model is nonlinear, the ReLu is a reliable activation function for this scenario. The Sigmoid activation function was chosen for the output for its capability of prediction target.

<img width="619" alt="ann8" src="https://user-images.githubusercontent.com/106359564/228977525-67279560-1f47-47df-a613-26c7aa060168.png">


o	My original model was only able to receive an accuracy score of 72.5%. After making changes for my second attempt, I was able to achieve a target performance of over 75%. The final accuracy score of the model was 78%.

<img width="540" alt="ann9" src="https://user-images.githubusercontent.com/106359564/228978430-b073a1a3-0ba5-4f46-be34-e11b8611a7fb.png">
<img width="553" alt="ann10" src="https://user-images.githubusercontent.com/106359564/228979468-52b871d3-2af1-4840-9cfe-30677d588b27.png">


o	To improve the performance I dropped one less column "NAME" from the original model which dropped two columns that included "EIN and "NAME". I also decreased the number of values for "NAME" and "ASK_AMT". Lastly, I used three ReLu activation hidden layers. The first layer had 90 neurons, the second had 40, and the third had 10.

<img width="479" alt="ann1" src="https://user-images.githubusercontent.com/106359564/228981456-6e1b9992-a39e-4e9a-8d87-ea0119d85799.png">
<img width="570" alt="ann2" src="https://user-images.githubusercontent.com/106359564/228981465-e354fa5e-122a-4c96-9927-7c1984ebd435.png">
<img width="551" alt="ann3" src="https://user-images.githubusercontent.com/106359564/228981471-2382f53f-fdc3-4c53-b1f1-48499272358d.png">
<img width="668" alt="ann4" src="https://user-images.githubusercontent.com/106359564/228981477-547a5692-0e3e-4da7-9a23-7e2415d3154e.png">


## Summary
After testing out my machine-learning model with different configurations I was able to achieve a higher accuracy score by dropping less features, removing many unique values for 2 additional bins, and adding three hidden layers. Since this neural network required a long data preparation process, I would recommend using the Random Forest Classifier model to receive similar and faster accuracy results but with much less code.




