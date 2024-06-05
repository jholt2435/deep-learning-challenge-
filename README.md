# deep-learning-challenge-
Overview of the analysis: Explain the purpose of this analysis.


-The purpose of this analysis is to  train a machine learning model with two hidden layers on eight different features in order to predict whether or not a a project is a success or not from the perspective of a non-profit loaning money. A success is deemed by whether or not the business that received the loan used the money effectively. 

Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?

-The target of this model is the "IS_SUCCESSFUL" column of the dataset. We are training the model to determine whether or not the loan led to a successful project or not ie was the money used effectively. 

What variable(s) are the features for your model?

-The features of the model are the "application type", the businesses "affiliation", the "businesses classification", the businesses "use case", the type of "organization", the "status", "Income Amount", special considerations Y/N, and the  "ask amount" for the loan. 


What variable(s) should be removed from the input data because they are neither targets nor features?

-The "EIN" and the business name were dropped from the model entirely. 

Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?

-I tried four different tests using two different actication types. I used "tan h" and tried to train the model with 8 nodes in the first layer and 5 nodes in the second layer. I was getting an accuracy of 72.49. -I, then, increased the number of nodes to 16 and 10. However, this surprisingly, slightly decreased my accuracy to 72.27. I,then, decided to change the activation type to "relu". I tried relu with 16 nodes and 10 nodes again and then also with 32 nodes and  20  nodes. I got accuracy scores of 72.61 and 72.89. I then left the model with "relu" as my activation type and 32 nodes in the first layer and 20 in the second layer. This had the highest accuracy score, albeit by a small margin. 

Were you able to achieve the target model performance?
-I was not able to acheieve the target model performance of 75% accuracy. 

What steps did you take in your attempts to increase model performance?

- As outlined above I tried four different configurations. I increased the number of nodes and changed the activation type.
  
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
- This method of deep learning was fairly effective, however I was unable to get it to reach maximum performance. Furtheremore, it seemed that it was goign to be impossible to reach the target of 75% accuracy. It seems that a "feed forward" neural netowrk will have limitations in getting to 75% accuracy. Thus, to acheive this goal we will likely need a more complex neural network, using "random forest" might help increase the accuracy. This method aggregates different models and may in turn boost the model's accuracy. 
