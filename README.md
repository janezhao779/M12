# Credit Risk Classification
The classification problem of credit risk constitutionally imbalanced, the reason is that the healthy loan easily outnumber risky loan. we use logistic Regression to train and evaluate model with imbalanced classes,with using the datesets of historical lending activity from a lending service company to build a model to idetify the trusthiness borrowers.

First Step,after reading the data into DataFrame , Create label y from loan_status column, X DataFrame from rest of the columns.Split the data to training and testing set . using the variables value_counts and train_test_split .Second , create logistic Regression model, fit logistic Regression model by training data(X_train,y_train).save the prediction into X_test. calculate accuracy score,generate confusion matrix and print classsification report.thirdly,predict logistic Regression model with resampled training data. Use RandomOverSampler module to resample the data,Use LogisticRegression classifier and resample to fit the model and make prediction. the same process  ,calculate accuracy score ,confusion matrix and classification report.

the result from model 1
        pre       rec       spe        f1       geo       iba       sup

          0       0.99      1.00      0.85      1.00      0.92      0.86     18719
          1       0.91      0.85      1.00      0.88      0.92      0.83       665

avg / total       0.99      0.99      0.85      0.99      0.92      0.86     19384




the result from model 2

                   pre       rec       spe        f1       geo       iba       sup

          0       0.99      1.00      0.84      1.00      0.92      0.85     18653
          1       0.99      0.84      1.00      0.91      0.92      0.83       731

avg / total       0.99      0.99      0.85      0.99      0.92      0.85     19384

overall, from the two model classification report,the accuravy score pretty close, all has the precision 0.99 and recall scores 1. therefore we don't have any perference recomendation for this prediction.






 
