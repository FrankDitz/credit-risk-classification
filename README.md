# credit-risk-classification
This challenge required me to take data from a csv file, containing information on borrowers and their laons/repayment history, and prepare the data for interpretaion and extrapolation. To do this, I loaded in the data, set y equal to "loan_status" and x equal to the data frame without the "loan_status" column, checked the balance of the variables using the value_counts function, and split the data into training and testing. After this I fit a logistic regression model to the training data and saved the predictions of the testing labels by using X+test and the fitted model. It was then necessary to evaluate the model's performance using the accuracy score of the model, generating a confusion matrix, and printing out a classification report. After this the assignment wanted me to use the RandomOverSampler module to create a dataset with equal datapoints in the x and y categories. Then I used the LogisticRegression classifier to fit the model and make new predictions anmd again evaluate the model by the original model's standards and compare the performance of the new model to the old.
* Machine Learning Model 1:
    *Accuracy: healthy: 1.00 high-risk: 0.88
    *Precision: healthy: 1.00 high-risk: 0.87
    *Recall: healthy: 1.00 high-risk: 0.89
    *Analysis: The logistic regression model predicts a low-risk loan with 100% precision and      a high-risk loan with 87% precision. The overall balanced accuracy of the model is            sitting at 94%.
* Machine Learning Model 2:
    *Accuracy: healthy: 1.00 high-risk: 0.93
    *Precision: healthy: 1.00 high-risk: 0.87
    *Recall: healthy: 1.00 high-risk: 1.00
    *Analysis: The logistic regression model predicts a low-risk loan with 100% precision and      a high-risk loan with 87% precision. The overall balanced accuracy 94%.
The summary of both models is that we can accurately make models that give us pretty good insite on who will be a good person to lend money to and vice versa. The second model is the better model as it outperforms model 1's accuracy, precision, and recall values. This gives us more confidence in model 2 being the right model for the job. With this model we can be fairly confident in our choices when determining the risk loaning money to potential clients.