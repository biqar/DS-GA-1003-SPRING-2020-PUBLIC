# README

## Autograder instructions

- You are expected to upload predictions on the test set in a csv file, which will be automatically evaluated against original labels of the test set, and appropriate results will be returned  
- Maximum number of submissions allowed is 5. Don't forget to activate your best submission, amongst your all 5 submissions  
- During submission please keep the leaderboard name same as your group name  
- Make atleast one submission ASAP. Don't wait for the last moment to use all your submissions. Gradescope will be facing heavy load during the last moments, and you don't want yourself stuck and waiting for the autograder results. We will **NOT** be accepting any late submissions.  
- Only one person from a group should submit. Please add all the other members to the group while making submission on gradescope  

1) **Fake review detection**  
- Input file to be graded should be named as 'predictions.csv'  
- The number of rows in this file is same as the number of rows in test data (72165)  
- Rows should be ordered the same way in test dataset, ie in the ascending order of 'ex_id'  
- Each row is single float "score" of positive class (fake class). Here "score" is defined the same way "y_score" is defined in 
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html  
- Test set and a sample predictions file is given here - https://drive.google.com/drive/folders/1BWBlmG5_PWd9yzR1Y1L-D59qg_x1Cgac?usp=sharing   

2) **Extreme classification**  
- Input file to be graded should be named as 'predictions.csv'  
- The number of rows in this file is same as the number of rows in test data (2489)  
- Rows should be ordered the same way in test dataset, ie in the ascending order of 'ex_id'  
- Each row is comma-separated values of float "score" of corresponding label. There are 3993 columns in each row.  
- For example, value in column 0 denotes the score of class 0. Here "score" is defined the same way "y_score" is defined in 
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.label_ranking_average_precision_score.html  
- There could be some classes/labels in the test set that don't occur in the training set  
- Test set and a sample predictions file is given here - https://drive.google.com/drive/folders/1eaonXJkuCGdXZkRJMUBnMrBNqberkPY6?usp=sharing  

Please note -  
1) Since prediction.csv will be a large file (~100MB) for extreme classification project, it might take a long time to upload the submission. A preferred approach is to first push this file to a github repository, and then submit the file through github. This is significantly faster than uploading the file through gradescope interface.  
2) It might take few minutes (< 10 mins) for gradescope to evaluate your submission. Please be patient.  
3) Should you have any questions, please post on piazza.  
Happy hacking!
