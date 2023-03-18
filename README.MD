

## A collection of Machine learning models built with Pycaret.

###  Models include 
1.  Superviced learning:  Regression and Classification (Binary 0 and 1) and 
2.  Unsuperviced leaning:  (Clustering)

### Datasets include

### Superviced
1.   Regression:   concrete production, predicting continuous. values
2.   Regression: House prices, predicting continuous values
3.   Classification : Penguins (0 and 1 Binary) where we predict the Pengiuns' Specie
4.   Classification : Diabetes detection  (0 and 1 Binary) where we predict if the person has diabetis or not


### Unsuperviced 
1.   Penguins(Clustering) detemining or guessing the bengine breeds based on features 


###  Pycaret Notes

```
## Env pip-310PC  gbc and gbr for classification

### https://github.com/pycaret/datasets/tree/main/data/common for pycaret datasets

### https://towardsdatascience.com/pycaret-3-0-is-coming-soon-whats-new-e890e6a69ff5
### https://www.kaggle.com/general/329102


```
#### Min Max Function
```

def minmax(x):
    return pd.Series(index=['min', 'max','mean','cleanQtile'], data=[x.min(), x.max(),x.mean(),x.quantile(q=0.75) - x.quantile(q=0.25)])
df.apply(minmax).T

```
```
beta_model['pct_err'] = (abs(beta_model['strength'] - beta_model['prediction_label'])) / beta_model['strength']

```