# sklearn_json
A python library to convert json represented ML model into scikit-learn classifier.

This library is based on json represented [machine learning model protobuf schema] (https://github.com/kellrott/ml-schema/blob/master/proto/ml_schema.proto).
It takes a json file as a parameter, and returns a scikit learn classifier. It supports Linear SVC, Linear Regression, and Logistic Regression.

### Usage
```
import sklearn_json
from sklearn.linear_model import LinearRegression

lr = LinearRegression()
lr.from_json('path/to/json')

lr.predict(data_to_apply_model)
```
