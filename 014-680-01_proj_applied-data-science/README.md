# 014-680-01_proj_applied-data-science.ipynb

Exploring Policies to Curb the Rate of Stomach Cancer in the ROK

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
import warnings
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
from sklearn.decomposition import PCA
import seaborn as sns
import sklearn
from functools import reduce
```

## Usage

```
dt01_cancer_incidents_______00 = pd.read_csv('암발생건수및현장별발생률24항목성별연령군_20240614155136.csv')
dt02_rates_death____________00 = pd.read_csv('원인별사망및사망률104항목성별연령별5년__20240614155018.csv')
dt03_stats_screening________00 = pd.read_csv('지역별성별별위암검진진단통계_20240614154803.csv')
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
