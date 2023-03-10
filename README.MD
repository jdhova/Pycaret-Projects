



## Pycaret Notes
## Env pip-310PC  gbc and gbr for classification

### https://github.com/pycaret/datasets/tree/main/data/common for pycaret datasets

### Min Max Function

```

def minmax(x):
    return pd.Series(index=['min', 'max','mean','cleanQtile'], data=[x.min(), x.max(),x.mean(),x.quantile(q=0.75) - x.quantile(q=0.25)])
df.apply(minmax).T

```