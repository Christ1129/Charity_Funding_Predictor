# Charity_Funding_Predictor

   The non-profit Alphabet Soup Foundation seeks to predict the best charity funding. Data containing over 34,000 organizations previously funded by Alphabet Soup and their metadata is preprocessed and fed into a deep learning neural network.
2 strategies were used:
•	a first in which the hyperparameters of the neural network are predefined and adjusted to the data (accuracy of 73%) and
•	a second optimized in which the hyperparameters were systematically tested used the keras tuner (accuracy of 77%)

### RESULT
Data Processing
•	EIN and NAME features were dropped from the model.
•	The model's target variable is IS_SUCCESSFUL. APPLICATION data was analyzed and CLASSIFICATION value was used for grouping
•	Each unique value used several data point as a cutoff point to bin categorical variables together in a new value. Categorical variables were encoded by “pd.get_dummies() ”.

 ### COMPILING, TRAINING, AND EVALUATING THE MODEL
 

 <img width="662" alt="define model" src="https://user-images.githubusercontent.com/100292828/185767448-674065ad-69a8-4ee0-a68f-b18034d25152.png">

-	As can be seen in the table below, 537 parameters were generated and the model accuracy was achieved at 73%

 
 <img width="388" alt="params" src="https://user-images.githubusercontent.com/100292828/185767669-69075b04-1193-435b-97dd-0efdaae400fc.png">
<img width="463" alt="evaluate" src="https://user-images.githubusercontent.com/100292828/185767509-03aaa105-b789-4957-95ae-54fe20aad55e.png">

 
 
### OPTIMIZATION
-	With hyperparameter optimization, the model was able to perform at 77%, which is 2 basis points better than 75%.

<img width="391" alt="optmz params" src="https://user-images.githubusercontent.com/100292828/185767619-84b7c5bc-398a-45d3-99e7-607d1193ba3b.png">
<img width="470" alt="optmz eval" src="https://user-images.githubusercontent.com/100292828/185767648-780f9301-eb8b-41fb-b241-5a8c3c5e3165.png">
 
 
### SUMMARY
Thanks to the results obtained, the neural model demonstrated decent reliability in predicting the success of charitable organizations. In this sense, Alphabet Soup obtains additional information about charities to fund in the future. You can test other optimizations to be carried out in the future (different pre-processing, additional data, etc.); additional tests (model variance test to check for overfitting) to check the power of the model.
I would suggest applying a PCA and/or tSNE model during the pre-processing step to reduce the number of features.

<hr>
Contact : 

* tourteau.christian@gmail.com
* https://www.linkedin.com/in/christian-tourteau/

