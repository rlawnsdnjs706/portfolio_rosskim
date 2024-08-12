# 680-03_proj_applied-data-science.ipynb

Exploring ways to curb the suicide rate in the Republic of Korea

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.metrics import silhouette_score
from sklearn.preprocessing import StandardScaler
import seaborn as sns
from sklearn.decomposition import PCA
from sklearn.cluster import KMeans
from datetime import datetime
import time
import numpy as np
import warnings
warnings.filterwarnings("ignore")
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
from pandas import read_csv
from pandas import DataFrame
from statsmodels.tsa.arima.model import ARIMA
from matplotlib import pyplot
from statsmodels.tsa.stattools import adfuller
import plotly.express as px
from sklearn.experimental import enable_hist_gradient_boosting
from sklearn.ensemble import HistGradientBoostingClassifier
from sklearn.datasets import make_classification
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
from sklearn.model_selection import cross_val_score, RepeatedStratifiedKFold
from numpy import mean, std
import xgboost as xgb
from xgboost import XGBClassifier
from lightgbm import LGBMClassifier
import sys
import time
import traceback
from joblib.externals.loky import set_loky_pickler
from joblib import Parallel, delayed
from joblib import wrap_non_picklable_objects
import multiprocessing as mp
from dask import dataframe as df1
import csv
from pyspark.sql import SparkSession
from sklearn.neighbors import KNeighborsClassifier
from sklearn import preprocessing
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, classification_report
from sklearn.linear_model import Ridge
```

## Usage

```
dt04_combined________________00 = pd.read_csv('combined_processed_data.csv')
dt05_stress_general__________00 = pd.read_csv('Degree_of_Stress__General_Life__13_years_old_and_over__20240719092712.csv')
dt06_stress_home_____________00 = pd.read_csv('Degree_of_Stress__Home_Life__13_years_old_and_over__20240719092914.csv')
dt07_stress_school___________00 = pd.read_csv('Degree_of_Stress__School_Life__13_years_old_and_over__20240719092757.csv', encoding = 'unicode_escape')
dt08_stress_work_____________00 = pd.read_csv('Degree_of_Stress__Work_Life__13_years_old_and_over__20240719092838.csv')
dt09_drinking_19_____________00 = pd.read_csv('Drinking__19_years_old_and_over__20240719093320.csv')
dt10_drinking_20_____________00 = pd.read_csv('Drinking__20_years_old_and_over__20240719093241.csv')
dt11_drinking_manage_19______00 = pd.read_csv('Drinking_and_Health_Management__19_years_old_and_over__20240719093528.csv')
dt12_drinking_manage_20______00 = pd.read_csv('Drinking_and_Health_Management__20_years_old_and_over__20240719093453.csv')
dt13_suicide_impulse_________00 = pd.read_csv('Impulse_to_Commit_Suicide_and_Reasons__13_years_old_and_over__20240719092337.csv')
dt14_suicide_impulse_________00 = pd.read_csv('Impulse_to_Commit_Suicide_and_Reasons__13_years_old_and_over__20240719092337.csv')
dt15_suicide_reason__________00 = pd.read_csv('Reason_and_Attempt_to_Think_Suicide_by_General_Feature_of_older_persons_Over_65_Years_Old__20240719092517.csv', encoding = 'unicode_escape')
dt16_suicide_reason__________00 = pd.read_csv('Reason_and_Attempt_to_Think_Suicide_by_General_Feature_of_older_persons_Over_65_Years_Old__20240719092517.csv', encoding = 'unicode_escape')
dt17_smoke_drink_19__________00 = pd.read_csv('Smoking_and_Drinking__19_years_old_and_over__20240719093138.csv')
dt18_smoke_drink_20__________00 = pd.read_csv('Smoking_and_Drinking__20_years_old_and_over__20240719093056.csv')
dt19_ph_categories___________00 = pd.read_csv('ph_categories_index.csv')
dt20_ph_analysis_____________00 = pd.read_excel('ph_Pornhub Analysis year by year.xlsx')
dt21_ph_videos_______________00 = pd.read_csv('ph_videos.csv')
dt22_ph_tot__________________00 = pd.concat(chunk)
dt23_408_03__________________00 = pd.read_csv('408_DT_40803_N0003_20240801134720.csv')
dt24_408_04__________________00 = pd.read_csv('408_DT_40803_N0004_20240801134840.csv')
dt25_index_eco_sent__________00 = pd.read_csv('Economic_Sentiment_Index_20240801135039.csv')
dt26_sadness_________________00 = pd.read_csv('Feeling_sad_or_hopeless_20240801134129.csv')
dt27_happiness_01____________00 = pd.read_csv('happiness.csv')
dt28_happiness_2015__________00 = pd.read_csv('index_happiness_2015.csv')
dt29_happiness_2016__________00 = pd.read_csv('index_happiness_2016.csv')
dt30_happiness_2017__________00 = pd.read_csv('index_happiness_2017.csv')
dt31_happiness_2018__________00 = pd.read_csv('index_happiness_2018.csv')
dt32_happiness_2019__________00 = pd.read_csv('index_happiness_2019.csv')
dt33_pop_income______________00 = pd.read_csv('Population_by_income_level_20240801133314.csv')
dt34_stress_perc_____________00 = pd.read_csv('Preceived_stress_20240801134258.csv')
dt35_suic_reason_____________00 = pd.read_csv('Reason_and_Attempt_to_Think_Suicide_by_General_Feature_of_older_persons_Over_65_Years_Old__20240801134427.csv', encoding='unicode_escape')
dt36_depr_symptom____________00 = pd.read_csv('Symptom_of_Depression_by_General_Feature_of_older_persons_Over_65_Years_Old__20240801135254.csv', encoding='unicode_escape')
dt37_happiness_world_________00 = pd.read_csv('World Happiness Report.csv')
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
