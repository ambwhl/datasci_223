Explain your choices, process, and outcomes.
All process performed using CPU on google colab

For task1: Classify all symbols
1. I chose RandomForestClassifier for this task as it has been considered able to handle high-dimensional data well because individual trees are trained on random subsets of the features.
2. 1000 training data and 1000 test data were loaded from emnit training and test sets respectively.
3. trained and tested RandomForestClassifier. n_estimators at this step was set as 50 to avoid system crash due to insufficient RAM. Performance Metrics showed that model was not very good:accuracy 0.549.
4. To investigate subsets, only digits data were subsetted from eminit and tran/test RandomForestClassifier. Performance Metrics showed that this classifier did better in digits data with accuracy of 0.875576. 
5. To improve performance, n_estimators was set as 100 and trained/tested with subsets in 4. Performance Metrics showed improved accuracy of 0.887097.
   
For task2:Classify digits vs. letters model showdown
1. Create a column for whether each row is a digit or a letter on data subsets from task1.
2. Estalish new display function.
3. Choose Logistic Regression as evaluation metric and trained/tested. Performance Metrics showed accuracy 0.675 
4. To compare,random forest also trained/tested using the same datasets and schema, Performance Metrics showed accuracy 0.78.
5. To performa k-fold train/test, original train/sets were combined and deivided into non-validation and validation sets. non-validation was further divided into 3 train/test sets:round1,round2 and round3.
6. Random forest and Logistic Regression were used on round1,2,3 respectively. Performance Metrics showed while Random forest is sensitive to sample sata and can have higher accuracy.  
7. I chose Random forest on validation data. Performance Metrics showed accuracy 0.56, suggestting that the model is struggling,likely due to the small size of the dataset and the possible absence of certain labels from the training set.
