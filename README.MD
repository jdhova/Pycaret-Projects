

##  A collection of Machine learning models built with Pycaret.
## Models include Superviced (Regression and Classification (Binary 0 and 1)) and Unsuperviced leaning models (Clustering)
## Datasets include

## Superviced
### House prices and concrete production for Regression
### Penguins (with the specie as a terget we are predicting a binary if we can  train the model to guess the penguin specie)
###  Diabetes detection for Clustering (0 and 1 Binary) based on the db we are predicting of the person is diabetic or not


## Unsuperviced 
### Penguins(Clustering) detemining or guessing the bengine breeds based on features 


###  Pycaret Notes

```
## Env pip-310PC  gbc and gbr for classification

### https://github.com/pycaret/datasets/tree/main/data/common for pycaret datasets

### https://towardsdatascience.com/pycaret-3-0-is-coming-soon-whats-new-e890e6a69ff5
### https://www.kaggle.com/general/329102


```
### Min Max Function
```

def minmax(x):
    return pd.Series(index=['min', 'max','mean','cleanQtile'], data=[x.min(), x.max(),x.mean(),x.quantile(q=0.75) - x.quantile(q=0.25)])
df.apply(minmax).T

```
```
beta_model['pct_err'] = (abs(beta_model['strength'] - beta_model['prediction_label'])) / beta_model['strength']

```