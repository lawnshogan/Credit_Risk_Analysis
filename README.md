# Credit Risk Analysis

##  **Project Overview**
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.  Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.


##  **Purpose**
1. Explain how a machine learning algorithm is used in data analytics.
2. Create training and test groups from a given data set.
3. Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
4. Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
5. Compare the advantages and disadvantages of each supervised learning algorithm.
6. Determine which supervised learning algorithm is best used for a given data set or scenario.
7. Use ensemble and resampling techniques to improve model performance.


### **Naive Random Oversampling**
- Balanced Accuracy: 0.6515938052705158
- Precision: Low for high-risk loans + high for low-risk loans
- Recall: High/Low Risk = .62/.68

### **Undersampling**
- Balanced Accuracy: 0.6241876870888075
- Precision: Low for high-risk loans + Low for low-risk loans
- Recall: High/Low risk = .59/.43

### **Combination Under & Over Sampling**
- Balanced Accuracy: 0.5102725100821478
- Precision: High for high-risk loans + High for low-risk loans
- Recall: High/Low risk = .70/.58

### **Balanced Random Forest Classifier**
- Balanced Accuracy: 0.7877672625306695
- Precision: Low for high-risk loans + high for low-risk loans
- Recall: High/Low risk = .67/.91

### **Easy Ensemble AdaBoost Classifier**
- Balanced Accuracy: 0.925427358175101
- Precision: High for high-risk loans + high for low-risk loans
- Recall: High/Low risk = .91/.94

##  **Summary**
1. Balanced Accuracy - The highest accuracy comparisons between 0 and 1 - The closest to 1 is the best machine learning model
2. Easy Ensemble AdaBoost Classifier is the best model to choose with its .925 balanced accuracy
3. The precision for all models were similar