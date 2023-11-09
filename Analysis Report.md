#Report on Alphabet Soup Prediction Model


##Overview of the Analysis

The primary objective of this analysis was to construct and evaluate a deep
learning model capable of predicting the success of charitable organizations in
receiving funding. Alphabet Soup, a philanthropic foundation, seeks to employ this
model to discern patterns within their historical data that can inform their
decision-making process.


#Results


##Data Preprocessing

Target Variable: The model's target variable was 'IS_SUCCESSFUL', indicating
whether the charity was successful in receiving funding.
Feature Variables: Features included various categorical and numerical data points
related to the application's characteristics, such as 'APPLICATION_TYPE',
'CLASSIFICATION', and others that potentially influence funding
success.
Variables Removed: Non-informative identifiers such as 'EIN' and 'NAME' were
removed as they do not contribute to the model's predictive ability.
Compiling, Training, and Evaluating the Model



##Neurons and Layers: 

The neural network model initially consisted of layers with 80
and 30 neurons respectively. The architecture was later optimized to include 90
neurons in the first layer and additional variations of neurons across subsequent
layers manually for the chance to achieve higher accuracy.
Activation Functions: 'ReLU' was chosen for its efficiency and effectiveness in
hidden layers, while 'Sigmoid' was used in the output layer due to the binary
nature of the classification task.
Model Performance: The target performance was an accuracy greater than 0.75. The
model achieved an accuracy of 0.72 initially, which improved to 0.73 after
optimization.

##Performance Improvement Steps:

Adjusting the number of neurons and layers.
Implementing Leaky ReLU activation functions.
Introducing Dropout layers for regularization.
Hyperparameter tuning with Keras Tuner.

##Summary

The deep learning model demonstrated a capacity to learn and predict funding
success to a certain extent. However, the improvement in accuracy through various
optimization techniques was marginal. Furthermore, the ultimate version of model
could not be sufficient, in a sense that 75% accuracy was not achieved.

##Recommendation for Alternative Model

Given the results, it is recommended to explore a Random Forest Classifier for this
classification problem for the following reasons:
Non-Linear Relationships: Random Forest can capture complex, non-linear
interactions between features without the need for extensive feature engineering.

##Feature Importance: 

It provides an intrinsic method for feature importance, offering valuable insights
into which features most influence the prediction.
Overfitting: Random Forest is less prone to overfitting, especially with the use of
ensemble strategies like bagging.
Ease of Use: It requires less hyperparameter tuning compared to deep learning
models, making it a practical choice for a quicker turnaround.

##Further Actions

To implement the Random Forest model, the following steps are suggested:
Analyze feature importance to identify the most predictive features.
Experiment with different ensemble strategies, such as boosting and stacking, to
enhance the Random Forest model.
Conduct cross-validation to ensure the model's robustness and generalizability.
The transition to a Random Forest Classifier could potentially yield a more
accurate and interpretable model for Alphabet Soup's funding success prediction,
aiding in more strategic decision-making.
