# Car Evaluation

Data location: https://archive.ics.uci.edu/ml/machine-learning-databases/car/car.data

The data analysis of the publically available car evaluation dataset linked above was performed in Python. The data was wrangled in order to scale values such as 'good' or 'high' and normalize some numerical values that refer to classification that was more 'string' in nature (ex: 2 doors).

While comments can be found to explain the coding, a list of procedure can be summarized below:
1) Load dataset as pandas dataframe, shifting the index to start at 1 and naming the columns appropriately.
2) After viewing the dataset, the string values were converted into a numerical scale and replaced in the dataframe.
3) Split the data into test and training data via sklearn.model_selection and perform kfold cross validation.
4) In viewing the data, it can be seen that regression trees are the most accurate prediction model.
5) A CART was created by sklearn.tree and the resulting tree is displayed.
6) Predicted car 'value' was determined for the X test data
7) Accuracy of the predicted 'values' compared to the Y test data was calculated
8) Incorrectly predicted values and their corresponding index value in the dataset are collected and displayed
