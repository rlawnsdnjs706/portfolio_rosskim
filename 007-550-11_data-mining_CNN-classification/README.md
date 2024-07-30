# 550-11_data-mining_CNN-classification.ipynb

CNN Classification

## Installation

Use the package manager [https://www.python.org/downloads/release/python-3109] to install Python.

```
from sklearn.metrics import confusion_matrix
import numpy as np
from keras.datasets import mnist
import matplotlib.pyplot as plt
from keras import layers
from keras import models
from keras.utils import to_categorical
```

## Usage

```
(img_trn, lbl_trn), (img_tst, lbl_tst) = mnist.load_data()
```

## Contributing

Pull requests are welcome. Please do not request changes of the original file.

Please make sure to update tests as appropriate.

## License

(www.ceroray.com)
