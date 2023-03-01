# Neural_Network_Charity_Analysis_Challenge-20

## Overview of the analysis
The project is aimed to predict whether applicants will be successful if funded by Alphabet Soup by using the features in the network charity dataset and establishing the machine learning model. 

## Results

### Data Preprocessing
- What variable(s) are considered the target(s) for your model?

The target for the model is IS_SUCCESSFUL. Because the purpose of the analysis is to predict whether the applicants will be sucessful if funded by Alphabet Soup. 

- What variable(s) are considered to be the features for your model?

In the original model, the variables that are considered to be the features for the model are application type, classification,use case, status, organization, income classification, special consideration and funding amount requested. 

In the optimized model, the variables that are considered to be the features for the model are name, application type, classification,use case, organization, income classification, special consideration and funding amount requested. 

- What variable(s) are neither targets nor features, and should be removed from the input data?

In the original model created, the identification columns (EIN and NAME) are removed from the input data. 

In the optimized model, the EIN and STATUS are removed from the input. 

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?

In the neural network model I created, there are four hidden layers. The number of neurons in the four hidden layers are 100, 80, 40, and 30, respectively. The activation function of the four hidden layers is relu. The activation function of the output layer is sigmoid. The reason of this selection is that the model performs better and the accuracy of performance has been improved. 

Since there is no easy solution or rule of thumb to identify how many layers are required to maximize performance, the only way to determine how "deep" the deep learning model should be is through trial and error. Through training and evaluating a model with increasingly deeper and deeper layers, the model demonstrates noticeable improvements over the same number of epochs.


- Were you able to achieve the target model performance?

Yes, the target model performance has achieved. The accuracy rate is 0.78, which is above 0.75. 

- What steps did you take to try and increase model performance?

(1) The additional STATUS column is dropped from the dataset and the NAME column is used as the features to train the model. 
(2) Create binns for NAME Columns because the frequency of applicants funded has connection with the prossibility of success of funding. 
(3) Decrease the number of values for bins of applicants and classification 
(4) add more hidden layers 
(5) add more neurons 
(6) increase the epochs 

### Summary
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
