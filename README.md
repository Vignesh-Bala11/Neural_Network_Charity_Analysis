# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis to determine which companies should recieve loans from Alphabet Soup using a neural network.

## Results 

   Data Preprocessing:

   After looking at the data, I established that the target variable is the "IS_SUCCESSFUL" column. I then removed the "EIN" and "NAME" columns as they did not offer any relevant data that could help the model perform better. The remaining columns became the features for the model.

    Compiling, Training and Evaluating the Model:

   The initial model consisted of 8 neurons in the first layer and 5 in the second layer. Both layers used the "relu activation function and the output layer used the sigmoid activation layer. The preformance for the metrics are as follows:
   
   ![og](https://user-images.githubusercontent.com/57723459/125206289-887dad00-e254-11eb-8576-d6981e192cf2.png)



   Optimization Attempt 1:

   The first attempt to increase the acccuracy of the model was to increase the number of trainable parameters. In order to do this I changed the first layer of neurons to a 100 and the second layer to 60. This changed the number of trainable paramters to 10, 521. The preformance for this iteration are as follows:
   
   
   
   ![optim_1](https://user-images.githubusercontent.com/57723459/125206301-95020580-e254-11eb-80e7-a4ef29a635fc.png)



   Optimization Attempt 2:

   Given the increase in accuracy I decided to keep the amount of neurons in the first and second layer as in the first optimization attempt, but decided to create a third layer which has 40 neurons. The preformance for this iterations are as follows:
   
   
   ![optim_2](https://user-images.githubusercontent.com/57723459/125206315-9e8b6d80-e254-11eb-9ceb-f7c24ad060fd.png)



   Optimization Attempt 3:

   In my final attempt to increase the acccuracy to over 75% I changed the activation functions for the three hidden layers and the output layer to selu. The preformance for this iterations are as follows:
   
   
   ![optim_3](https://user-images.githubusercontent.com/57723459/125206324-a77c3f00-e254-11eb-9357-2983b59d3734.png)



# Summary
After these 4 attempts the I was unable to create a model that achieved 75% accuracy. I believe that after the first 2 attempts there were increases in accuracy but changiing the activation function caused there to be significant accuracy drop off. I believe to get the model to 75% accuracy would involve re-assessing the dataset and training the model using different labels. Also work would be undertaken in determining the best activation function. 
