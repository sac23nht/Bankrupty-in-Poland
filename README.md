# Gradient Boosting Modeling of the Poland Bankruptcy Dataset
This notebook demonstrates the implementation of Gradient Boosting as an ensemble model to predict bankruptcy in the Poland bankruptcy dataset.

Gradient Boosting is an ensemble model that combines the predictions of multiple weak learners (usually decision trees) to create a stronger model. It is an iterative process that trains new weak learners on the residual errors of the previous learners. The final prediction is the weighted sum of all the weak learners.

# Data Preprocessing
The first step was to split the dataset into testing and training sets. The training set was used to train the model, while the testing set was used to evaluate the model's performance.

Next, I used the oversampling technique to address the class imbalance issue in the dataset.

# Model Creation
In the iterative section, a Gradient Boosting Classifier was created using a Simple Imputer transformer and Gradient Boosting Classifier predictor. After some hyperparameter tuning, the model was created using the classifier and hyperparameter grid.

Cross-validation results were extracted from the model and used to create a DataFrame. The best hyperparameters were extracted, and the training and validation accuracy scores were evaluated.

# Evaluation
Finally, I evaluated the model's performance using a confusion matrix and classification report. An interactive dashboard was also created to visualize the model's predictions.