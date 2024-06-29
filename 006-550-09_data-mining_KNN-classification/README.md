# 006-550-09_data-mining_KNN-classification.ipynb

KNN Classification

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.pipeline import Pipeline
from sklearn.preprocessing import MinMaxScaler
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.neighbors import KNeighborsClassifier
from sklearn.model_selection import GridSearchCV
import os
os.environ["OPENBLAS_NUM_THREADS"]= "1"
```

## Usage

```
dt01 = pd.read_csv('Loan_Train.csv')
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
