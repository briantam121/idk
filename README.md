# Logistic Regression

Logistic Regression is a algorithm to predict a categorical results.


## Usage

### Initilize data
```python
#import libraries
import pandas as pd
import numpy as np
#read .csv file
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

### Initilize Logistic Regression
```python
# learning_rate and n_iters is learning rate and number of iterations respectively
# default value of learning_rate n_iters and is 0.01 and 1000 respectively
# both of them are optional
lgr = Logistic_Regression(learning_rate = 0.01,n_iters=1000) 
```

## License
Name: Tam Pa Yan 
UID: 3035573874
