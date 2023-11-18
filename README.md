# Challenge-20
In this Assignment, the Logistic Regression model was implemented on the Loan dataset to predict high risk loans and healthy loans both without alterations to the dataset, as well as with Random OverSampler to overbalance the minority class of high risk loans in order to increase precision and accuracy of the model by giving it more examples. The initial result revealed that high risk loans were predicted with precision of 85%, meaning that 15% of the time the predictions were incorrect. The revised dataset with RandomOverSampler on the minority class of the high risk loans showed the predictions with 99% accuracy for both the high risk and healthy loans. 

I believe this model should be used as a preliminary framework for the problem, as it is the correct model type for the problem at hand - classification with logistic regression, given that we are predicting two classes of loans. I would recommend including Standard Scaler, which would convert all of the columns to the same scale, and additional modeling techniques, such as hyperparameter tuning, where the optimal parameters are identified with GridSearchCV implementation. 

In the real world, the datasets may require extensive preprocessing, including revision of variables to get the data in the right format for the model and the codes for the preprocessing can get complex with extensive conversions. A range of algorithms should be implemented on the model including Deicision Tree Classifier and Random Forest Classifier, with a comparison of the classification report across the models, as well as Gradient Boosting Classifier and Adaboost, which are more complicated machine learning algorithms that examine an extenesive set of weak learner models and weigh their predictions for the final vote. 

In Summary, the Classifications Reports indicated the following trends:
- The precision score was higher for healthy loans than for high risk loans in initial implementation.
- After overweighing the minority high risk loan class to ensure that the model can have sufficient examples to detect the patterns, the precision and accuracy scores for the two classes were equal at 99%.
