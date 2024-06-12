# min-sklearn

<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

We build a tiny core subset of `scikit-learn` from scratch for
educational purposes, with the same API.

The only dependency is `numpy` (so far).

## Install

Clone this repo and

``` bash
pip install -e .
```

`-e` for editable mode.

## How to use

``` python
from min_sklearn.metrics import accuracy_score
import numpy as np
```

``` python
x = np.array([0, 1, 2, 3])
y = np.array([0, 1, 2, 5])
assert accuracy_score(x,y, normalize=True, sample_weight = np.array([1, 1, 1, 0])) == 1.0
```
