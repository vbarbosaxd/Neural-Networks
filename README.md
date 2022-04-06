# Neural Networks
## Overview of the analysis: 
A nonprofit organization wants to create a model that helps accurately predict whether or not applicants will be successful if they receive funding from the organization AlphabetSoup.
## Results
### Data Preprocessing 
What variable(s) are considered the target(s) for your model?
* IS_SUCCESSFUL – whether or not the funding money was used effectively

What variable(s) are considered to be the features for your model?
*	APPLICATION_TYPE - application type
*	AFFILIATION - affiliated sector of industry
* CLASSIFICATION  - government organization classification
*	USE_CASE - use case for funding
*	ORGANIZATION - organization type
*	STATUS - active status
*	INCOME_AMT - income classification
*	SPECIAL_CONSIDERATIONS - special consideration for application
*	ASK_AMT - funding amount requested

What variable(s) are neither targets nor features, and should be removed from the input data?
*	EIN – ID of applicant
*	NAME – name of applicant
### Compiling, Training, and Evaluating the Model 
How many neurons, layers, and activation functions did you select for your neural network model, and why?
*	For my base model, I selected two layers with 5 neurons each using the Relu and Sigmoid activation functions, because this is the basic setup we used in class activities, so I wanted to see how the model would react with these basic inputs  

Were you able to achieve the target model performance?
*	No, even though I tried dropping more columns, increase the number of hidden layers, and decrease the number of epochs

What steps did you take to try and increase model performance?
*	For my first attempt:
*	I increased the number of neurons for each layer, from five to ten 
*	Kept everything else the same
*	For my second attempt:
*	I increased the number of layers from two to three
*	I put eight neurons in the first layer
*	Five neurons in the second and third layer, and
*	Decreased the number of epochs to 50.
*	For my third attempt:
*	I dropped the columns “SPECIAL_CONSIDERATIONS_N”, “SPECIAL_CONSIDERATIONS_Y”, and “STATUS” to decrease noise
*	Used three layers
*	Put 10 neurons in the first layer,
*	Put 8 neurons in the second layer, and 
*	Put 5 neurons in the third layer
## Summary:  
Since the overall accuracy score was not above 75% with the neural networks model, we could use the Random Forest classifiers. This is because random forest is a robust and accurate model due to their sufficient number of estimators and tree depth. Also, the random forest models have a faster performance than neural networks and could prevent the data from being overfitted.

