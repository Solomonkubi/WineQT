## Wine Quality analysis
A mini project to analyze the quality of wine
# Getting started
To run this repo, the following  packages need to be imported;
import pandas as pd 
import numpy as np
import scipy as scp
import seaborn as sns
import matplotlib.pyplot as plt

# Read and load the file
wine_datatset = pd.read_csv('WineQT.csv', header=0)
# Load only the first 1000 rows
wine_datatset.head(100)

# gives basic statistics of dataframe
wine_datatset.describe()

wine_datatset[['fixed acidity', 'quality', 'volatile acidity']]
# how can i get multiple columns

# checking the null values of the data
null_count = wine_datatset.isnull().sum().sum()
print(null_count)

null_count = wine_datatset.isnull().sum()
print('Number of null values:', null_count)

# a plot of wine quality and the frequency levels
sns.countplot(x='quality', data=wine_datatset, palette=['blue'] + ['red'] + ['yellow'])
plt.xlabel('Wine quality')
plt.ylabel('Frequency')
plt.title('Wine quality classes')
plt.show()

# Relation between volatile acidity vs quality
plot = plt.figure(figsize= (6,5))
sns.barplot(x='quality' , y= 'volatile acidity' , data= wine_datatset)
plt.title('volatile acidity and quality');
