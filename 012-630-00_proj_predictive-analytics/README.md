# 012-630-00_proj_predictive-analytics.ipynb

Exploring Policies to Stabilize Housing Prices in the ROK

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
import warnings
warnings.filterwarnings("ignore")
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
from sklearn.decomposition import PCA
import thinkstats2
import thinkplot
import datetime
import statistics
import first
from scipy.stats import poisson
from sklearn.preprocessing import PolynomialFeatures
import math
from sklearn.tree import DecisionTreeRegressor
from sklearn import tree, metrics
import pandas_datareader.data as web
import pandas_datareader as web
import seaborn as sns
from sklearn.preprocessing import MinMaxScaler
from sklearn.feature_selection import RFE
import statsmodels.api as sm
from statsmodels.stats.outliers_influence import variance_inflation_factor
from sklearn.feature_selection import SelectKBest
from sklearn.feature_selection import chi2
from sklearn.metrics import classification_report
from sklearn import model_selection
from sklearn.linear_model import LogisticRegression
from sklearn import preprocessing
from sklearn import utils
```

## Usage

```
dt01 = pd.read_csv('주택가격지수(매매)_20240320113224.csv')
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
