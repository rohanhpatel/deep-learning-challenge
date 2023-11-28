# Report

## Overview

This analysis will describe the neural network model I used to try to get to 75% accuracy on this dataset.

## Results

### Preprocessing

#### Targets

The variable that was the target for the model was whether or not the funding was successful.

#### Features

The features that were used was the income amount of the company, the goverment classification of the company, the use case for the funding, the affiliation of the company, and how much the company asked for.

#### Extra Variables

Certain variables, like whether or not a company had special considerations, or the company's active status, were very one sided and so these features were not used for the model.

### The Model

The architecture for the model is shown below.

1. 90 sigmoid
2. 110 relu
3. 95 relu
4. 50 relu
5. 20 relu
6. 1 sigmoid

This model gave an accuracy of 0.7371.

We were not able to achieve the desired 75% accuracy, however there was one or two models that were created along the way that were 74% accurate.

#### Steps

In attempting to increase the model's performance, I did several things, I:

1. Changed binning for income amount
2. Removed status and special considerations columns
3. Changed the original model architecture
4. Changed the number of epochs that the model trained for from 100 to 150

### Summary

To summarize, the deep learning model has potential, however I wasn't able to properly tune the hyperparameters to have a great model. Perhaps adding different types of layers like pooling layers and convolutional layers could have improved this model's performance.