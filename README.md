# Logistic Regression
Logistic Regression is a algorithm to predict a categorical results.


## Usage
### Initilize data
```python
#import libraries
import pandas as pd
import numpy as np
#read .csv file (iris data as example)
X_train = pd.read_csv("iris_X_train.csv")
X_test = pd.read_csv("iris_X_test.csv")
y_train = pd.read_csv("iris_y_train.csv")
y_test = pd.read_csv("iris_y_test.csv")
```
### Initilize Logistic Regression
```python
# learning_rate and n_iters is learning rate and number of iterations respectively
# default value of learning_rate n_iters and is 0.01 and 1000 respectively
# both of them are optional
lgr = Logistic_Regression(learning_rate = 0.01,n_iters=1000) 
```
### Using fit function
```python
# it will fit X_train and y_train data into the model
lgr.fit(X_train,y_train)
```
### Using score function
```python
# it will return the accuracy of model by predicting X_test result then compare to y_test
# it must use fit function before score function
lgr.score(X_test,y_test)
```
### Using predict function
```python
# it will return the predict result in form of numpy array
# it must use fit function before score function
lgr.predict(X_test)
# we can also use this method by input single and multiple rows of pandas dataframe
lgr.predict(X_test.loc[1])) # single prediction
lgr.predict(X_test.loc[0:2])) # multiple prediction
```

## License
Name: Tam Pa Yan 
UID: 3035573874
