Alphabet Soup Charity Success Prediction

Overview

This project develops a machine learning model using TensorFlow to predict the
success of charity organizations in receiving funding. The aim is to assist the
philanthropic organization, Alphabet Soup, in identifying the factors that
contribute to the success or failure of the funding applications they receive.

Data Preprocessing


The dataset provided includes various categorical and numerical features
representing the characteristics of the charity organizations and their funding
applications. The preprocessing steps involved:
Removing non-informative identifiers such as 'EIN' and 'NAME'.
Encoding categorical variables using one-hot encoding.
Grouping rare occurrences in categorical variables to reduce dimensionality.
Normalizing numerical features to ensure consistent scale.

Model Development


A deep learning model was constructed using TensorFlow's Keras API with the
following characteristics:
Multiple dense layers with a range of neurons.
Dropout layers to prevent overfitting.
Activation functions including ReLU, tanh, and sigmoid.

Optimization Process


Hyperparameter tuning was conducted using Keras Tuner with a focus on:
Number of neurons in each layer.
Number of hidden layers.
Activation functions for the hidden layers.
Learning rate for the Adam optimizer.
Dropout rate for each layer.
Callbacks like EarlyStopping and ReduceLROnPlateau were implemented to fine-tune
the training process.

Results


The initial model achieved an accuracy of 72%, which was incrementally improved
through hyperparameter tuning. Despite optimization efforts, the target accuracy of
75% was not attained, suggesting the need for further refinement or alternative
modeling approaches.
