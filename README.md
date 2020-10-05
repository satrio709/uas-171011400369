matplotlib inline
from pandas import Series, DataFrame
import pandas as pd
import numpy as np
import os
import matplotlib.pylab as plt
from sklearn.model_selection import train_test_split
from sklearn.metrics import classification_report
import sklearn.metrics
from sklearn import datasets
from sklearn.ensemble import RandomForestClassifier
data = pd.read_csv("file name")
data.head(10)
data.shape
data.isnull().sum()
data_clean = data.dropna()
num_of_numerical_cols = data_clean._get_numeric_data().columns.shape[0]
print(num_of_numerical_cols, 'numerical columns')
name_of_numerical_cols = data_clean._get_numeric_data().columns
print(name_of_numerical_cols)
