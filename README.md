# CIFAR-10_data
Python 2/3 compatible .npz CIFAR-10 dataset

The [official Python download for CIFAR-10 data](https://www.cs.toronto.edu/~kriz/cifar.html) uses .pickle format with a protocol that only supports Python 2.X. This is the same data compressed and saved in the .npz format. Load it from Python 2 or 3 with the following syntax

```python
import numpy as np
with np.load('cifar-10-python.npz') as data:
    out = tuple(data[k] for k in ['x_train', 'y_train', 'x_test', 'y_test'])
x_train, y_train, x_test, y_test = out
```
[Here](https://github.com/nickstanisha/CIFAR-10_data/blob/master/cifar-10-python.npz?raw=true) is a link to the raw download (240 MB).

![the data](data.png)
