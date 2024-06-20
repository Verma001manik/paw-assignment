# Introduction
This repo contains a jupyter notebook and a ppt for  PawScan.Ai . 

# Approach 
We used sklearn's DecisionTreeClassifier and use their accuracy_score for calculatiing the accuracy. At the end we got an overall accuracy of 74% . 
The entire dataset consisted of numerical columns except the dependent variable or the target that needs to be predicted ('Target'). 
So the consistent variables or the numerical values can be easily feeded to our model but as the target value is a string , we first need to convert the string into some
numerical form which will help in better predicting the values . 
For converting the target values into some numerical form we use LabelEncoding from sklearn library . There are 3 possible values for the 'Target' column . So the LabelEncoder will
convert each of them into [2...1...0...]. 
Graduate :2 
Dropout  :1       
Enrolled :0 
