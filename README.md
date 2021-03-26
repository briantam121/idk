# Logistic Regression
```
Logistic Regression is a algorithm to predict a categorical results.
```

## Usage
```
I used jupyer notebook with python language with this assignment.
Open the logistic_regression.ipynb to run the class cell first.
Then, types the following commands for creating logistic regression model.
```
### Initilize dataset (with continuous datasets)
```python
#import libraries
import pandas as pd
import numpy as np
#read .csv file (iris dataset as example)
X_train = pd.read_csv("iris_X_train.csv")
X_test = pd.read_csv("iris_X_test.csv")
y_train = pd.read_csv("iris_y_train.csv")
y_test = pd.read_csv("iris_y_test.csv")
```

### Initilize dataset (with catagorical datasets)
```python
#import libraries
import pandas as pd
import numpy as np

#read .csv file (car dataset as example)
X_train = pd.read_csv("car_X_train.csv")
X_test = pd.read_csv("car_X_test.csv")
y_train = pd.read_csv("car_y_train.csv")
y_test = pd.read_csv("car_y_test.csv")

# encoder function to create encoded dataset i.e. convert string data into categorical numeric values
# dummies function to create dummies dataset i.e. convert string data into categorical numeric arrays
# it will print the dictionary of X and y dataset
y_train,y_test = lgr.encoder(y_train,y_test)
X_train,X_test = lgr.dummies(X_train,X_test)
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
```
Name: Tam Pa Yan 
UID: 3035573874
```
