Explain your choices, process, and outcomes.
All process performed using CPU on google colab

For task1: Classify all symbols
1. I chose RandomForestClassifier for this task as it has been considered able to handle high-dimensional data well because individual trees are trained on random subsets of the features.
2. 1000 training data and 1000 test data were loaded from emnit training and test sets respectively.
3. trained and tested RandomForestClassifier. n_estimators at this step was set as 50 to avoid system crash due to insufficient RAM. Performance Metrics showed that model was not very good:accuracy 0.549.
4. To investigate subsets, only digits data were subsetted from eminit and tran/test RandomForestClassifier. Performance Metrics showed that this classifier did better in digits data with accuracy of 0.875576. 
5. To improve performance, n_estimators was set as 100 and trained/tested with subsets in 4. Performance Metrics showed improved accuracy of 0.887097.
For task2:Classify digits vs. letters model showdown
