# 550-07_data-mining_feature-selection.ipynb

Feature Selection

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
from sklearn import tree
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeRegressor
from sklearn.linear_model import LinearRegression
from sklearn import tree, metrics
import seaborn as sns
import math
from sklearn.preprocessing import StandardScaler
from sklearn.decomposition import PCA
from sklearn import datasets
from sklearn.datasets import load_digits
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
from sklearn.preprocessing import MinMaxScaler
from sklearn.utils import shuffle
import pickle
from sklearn import preprocessing
from sklearn.preprocessing import LabelEncoder, OneHotEncoder
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score
from sklearn.metrics import confusion_matrix
from sklearn.feature_selection import chi2
from sklearn.feature_selection import SelectKBest
```

## Usage

```
dt01 = open('WK07_data_description.txt', 'r')
print(dt01.read())
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
