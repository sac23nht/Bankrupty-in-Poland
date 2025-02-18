# Random Forest Modeling of Poland Bankruptcy Data
This Jupyter notebook demonstrates the Random Forest modeling of the Poland bankruptcy data. During the exploratory data analysis (EDA) phase, it was discovered that the data was imbalanced. To address this issue, both over and under-sampling resampling methods were attempted to see which would perform better for the model. Ultimately, the over-sampling method was chosen, as too much data was being discarded with under-sampling.

Given the imbalanced nature of the data, the training baseline was found to be quite high. Three identical models were then created: model_reg, model_under, and model_over. Each model utilized a SimpleImputer followed by a DecisionTreeClassifier. model_reg was trained using the unaltered training data, model_under was trained using the undersampled data, and model_over was trained using the oversampled data.

A confusion matrix was then added to assess the performance of each model. Finally, a bar chart was generated to identify the most important features (all of which are listed in the data dictionary). The model was then saved.


The notebook is structured in a way that's easy to follow and understand with notes to explain each step taken properly.

