# 004-550-05_data-mining_sentiment-analysis

Sentiment Analysis

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
import numpy as np
import pandas as pd
from sklearn.feature_extraction.text import CountVectorizer
from sklearn.feature_extraction.text import TfidfTransformer
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.linear_model import LogisticRegression
import csv
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.datasets import load_diabetes
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix, roc_curve, auc
from sklearn.naive_bayes import MultinomialNB
from sklearn import metrics
import nltk
import re
import string
from nltk.stem import WordNetLemmatizer
nltk.download('stopwords')
import seaborn as sns
%matplotlib inline
import warnings
from sklearn import linear_model
from sklearn.neighbors import KNeighborsClassifier
from sklearn.metrics import classification_report, confusion_matrix
from nltk.stem import PorterStemmer
from nltk.tokenize import word_tokenize
from sklearn.metrics import precision_score
```

## Usage

```
dt01 = pd.read_csv('labeledTrainData01.csv')
print(dt01.head())
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
