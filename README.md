Alphabet Soup Charity Success Prediction

Overview

The aim of this project is to develop a machine learning model using TensorFlow to predict the success of charity organizations in receiving funding. Our goal is to assist Alphabet Soup, a philanthropic organization, in identifying factors that influence funding application outcomes, helping them improve their decision-making process.

Data Preprocessing

The dataset provided includes both categorical and numerical features representing characteristics of charity organizations and their funding applications. Our data preprocessing involved:

Removing Non-informative Identifiers:

Eliminated features like 'EIN' and 'NAME,' which don't contribute to the predictive model.
Encoding Categorical Variables:
Applied one-hot encoding to categorical features.
Grouping Rare Occurrences:
Aggregated infrequently occurring categories to reduce dimensionality.
Normalizing Numerical Features:
Standardized numerical features to ensure a consistent scale.
Model Development
The predictive model was built using TensorFlow's Keras API, employing a deep learning architecture with the following key characteristics:

Multiple Dense Layers:

Each layer contains a range of neurons to capture complex patterns.
Dropout Layers:
Introduced dropout layers to mitigate overfitting.
Activation Functions:
Utilized a variety of activation functions, including ReLU, tanh, and sigmoid.
Optimization Process
To refine the model's performance, we used Keras Tuner to optimize hyperparameters, focusing on:

Number of Neurons & Layers:

Determined the optimal number of neurons and hidden layers.
Activation Functions:
Experimented with different activation functions for hidden layers.
Learning Rate:
Tuned the learning rate for the Adam optimizer.
Dropout Rate:
Adjusted the dropout rate for each layer.
Callbacks:
Implemented EarlyStopping and ReduceLROnPlateau to enhance the training process.
Results
Initially, the model achieved an accuracy of 72%. With iterative tuning, the performance improved, but the target accuracy of 75% was not attained. This suggests that further refinement or alternative modeling approaches are needed to meet the desired predictive accuracy.

Conclusion

While significant progress was made, future work should explore additional strategies like feature engineering, advanced architectures, or different machine learning models to achieve more reliable predictions.
