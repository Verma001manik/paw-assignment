# Introduction
This repo contains a jupyter notebook and a ppt for  PawScan.Ai . 

# Approach 
We used sklearn's DecisionTreeClassifier and use their accuracy_score for calculatiing the accuracy. At the end we got an overall accuracy of 74% . 
The entire dataset consisted of numerical columns except the dependent variable or the target that needs to be predicted ('Target'). 
So the consistent variables or the numerical values can be easily feeded to our model but as the target value is a string , we first need to convert the string into some
numerical form which will help in better predicting the values . 
For converting the target values into some numerical form we use LabelEncoding from sklearn library . There are 3 possible values for the 'Target' column . So the LabelEncoder will
convert each of them into [2...1...0...]. 
1) Graduate :2 
2) Dropout  :1
3) Enrolled :0 

After the initial predictions and measuring the accuracy of our model , we did some feature importance to know what columns really mattered in determining the result and only from finding the feature importance we got to know that there were roughly 2 most important columns that were directly related to the result . So we ended up removing all the columns except the important ones and trained again .

     
