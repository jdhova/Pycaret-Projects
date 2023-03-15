



## Pycaret Notes
## Env pip-310PC  gbc and gbr for classification

### https://github.com/pycaret/datasets/tree/main/data/common for pycaret datasets

### https://towardsdatascience.com/pycaret-3-0-is-coming-soon-whats-new-e890e6a69ff5
### https://www.kaggle.com/general/329102

### Min Max Function

```

def minmax(x):
    return pd.Series(index=['min', 'max','mean','cleanQtile'], data=[x.min(), x.max(),x.mean(),x.quantile(q=0.75) - x.quantile(q=0.25)])
df.apply(minmax).T

```
```
beta_model['pct_err'] = (abs(beta_model['strength'] - beta_model['prediction_label'])) / beta_model['strength']

```