# Neural_Network_Charity_Analysis

Utilizing deep learning netw to evaluate data for a nonprofit foundation, Alphabet Soup, to predict likeliness of a grantee being successfull. 

## Overview

The donor database from Alphabet Soup is being analyzed to see a decision making tool can be created to predict which grants will end in successful outcomes.  The data needed to be pre-processed, a model developed, compiled and trained to the model and finaly, the model evaluated in its effectiveness as a predictive tool. 

### Data Preprocessing
The first steps of data anlysis include review and preprocessing of the data so it can be used in the model. 

 - The target (variable of interest) is IS_SUCCESSFUL column.
 - The variables that are considered to be features in the model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
 - The variables that are considered to be neither targets nor features are EIN and NAME and they were removed from the input data. 

### Compiling, Training and Evaluating the Model

- The initial set up for the model was 80 neurons with a relu function for the first layer, 30 neurons for the second layer with a relu function and a sigmoid function for the outer layer. 
- During optimization efforts, I attempted the following changes: 
  -   Changed the hidden layer activation to "tanh"
  -   Added more neurons to the hidden layers (increased layer 1 to 100 and layer 2 to 50)
  -   Added a third hidden layers with 15 neurons 
-  I was unable to achieve the target model performance of 75%. The best performance achieved was adding the third hidden layer and a performance of 72.7% and loss of 0.55. 

### Summary
The non-essential featues were removed, the models were adjusted and the accuracy of the model in predicting the success of a grant did not meet the performance goals. 

### Recommendation

Additional exploration of the model should be conducted to determine which feature is impacting the desired outcome of IS_SUCCESSFUL.  It would be good to use the random forest model to evaluate the features and then further simplify the model so that the essential items are being used to fit the model and it will be more useful.  



