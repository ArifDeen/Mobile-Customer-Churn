CONTENTS OF THIS FILE
---------------------

* Introduction
* Requirements
* Description of fields
* Importing Recommended Modules



INTRODUCTION
------------
In this task you will work with some (fake but realistic) data on Mobile Customer Churn. Churn is where a customer leaves the mobile provider. The goal is to build a simple predictive model to predict churn from available features.

The data was generated (by Hume Winzar at Macquarie) based on a real dataset provided by Optus. The data is simulated but the column headings are the same. (Note that I'm not sure if all of the real relationships in this data are preserved so you need to be cautious in interpreting the results of your analysis here).

The data is provided in file MobileCustomerChurn.csv and column headings are defined in a file MobileChurnDataDictionary.csv (store these in the files folder in your project).

REQUIREMENTS
------------

- to build a simple predictive model to predict churn from available features
- finding out which features provide the most accurate results

IMPORTING RECOMMENDED MODULES
------------
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
from sklearn.impute import SimpleImputer
from sklearn.preprocessing import OneHotEncoder
from sklearn.compose import ColumnTransformer
from sklearn.feature_selection import SelectKBest
from sklearn.feature_selection import chi2
from sklearn.ensemble import ExtraTreesClassifier
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn import metrics
from sklearn.metrics import confusion_matrix
