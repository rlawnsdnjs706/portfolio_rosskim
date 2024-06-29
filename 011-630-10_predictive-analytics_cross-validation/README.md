# 011-630-10_predictive-analytics_cross-validation.ipynb

Cross Validation / Recommender

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error
from datetime import datetime
from surprise import Reader, Dataset, SVD
from surprise.model_selection import cross_validate
from sklearn.metrics import r2_score
import warnings
warnings.filterwarnings("ignore")
```

## Usage

```
dt01 = pd.read_csv('ratings.csv')
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
