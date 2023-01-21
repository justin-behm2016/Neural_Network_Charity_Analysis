# Neural_Network_Charity_Analysis
## Overview 
The goal of doing this neural network analysis was to help predict future investments. By creating a binary classifier for Alphabet Soup, key information on which applicants would achieve success with proper funding was gained. The dataset containing the organizations and various information about them was processed and funneled into a variety of neural models in an attempt to find a high accuracy for predicting success. 

### Results
Data Preprocessing
* The target values in this dataset were the "IS_SUCCESSFUL" values from the CSV file as we were trying to determine which loan applicants would be successful with funding.
* The features varied depending on the model; however, each model had the "EIN" and "NAME" features removed with some models also removing the "AFFILIATION" and "USE_CASE" features. Each model at least contained features such as "APPLICATION_TYPE", "CLASSIFICATION", "INCOME_AMT", etc.
* Some of the removable variables are as listed above, variables like "EIN" and "NAME" are neither targets nor features and were therefore removed from the input data.

Compiling, Training, and Evaluating
* Each model had variance in the setup regarding neurons, layers, and activation functions. For optimization model 2 the tanh activation was used with two hidden layers to attempt to get closer to the desired %75 accuracy. Optimization model 3 used the relu activation with three hiden layers. Optimization model 1 used 2 hidden layers with a higher number of neurons while maintaining the relu activation.
* Unfortunately, current model optimizations were unable to achieve the target model performance.
* Model performance was changed to try to increase accuracy levels accross all optimizations. Tanh was used instead of relu, additional hidden layers were added, additional columns were dropped from the dataset, and additional neurons were used when establishing the model.

#### Summary
The deep learning model was successfully established and a variety of models were tested with the data. Unfortunately, the target performance was not met with any of the current optimizations, thus leaving room for improvement. Moving forward, I would suggest further optimization of the model to continue to increase performance. I would recommend keeping the hidden layers at a maximum of 4 or 5 to attempt to reduce chances of overfitting and I would recommend trying to use a leaky relu activation to see if the further inclusion is able to increase performance. 
