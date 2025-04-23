#  Wine Quality Analysis
A mini data science project focused on analyzing the quality of wine using statistical methods and visualizations. The dataset contains physicochemical tests and quality scores of wine samples.

## Project Overview
This project explores relationships between various physicochemical attributes of wine (like acidity, sugar, and pH) and its quality. Through this analysis, we aim to draw insights and visualize trends that can help understand what makes a wine high or low quality.

## Getting Started
To run this project, ensure you have the following Python packages installed:
- import pandas as pd
- import numpy as np
- import scipy as scp
- import seaborn as sns
- import matplotlib.pyplot as plt
- You can install any missing libraries using pip:
pip install pandas numpy scipy seaborn matplotlib

## Data Loading and Exploration
Load the dataset:
wine_dataset = pd.read_csv('WineQT.csv', header=0)
Preview the first 100 records:
wine_dataset.head(100)

Get summary statistics:
wine_dataset.describe()

Select key features for analysis:
wine_dataset[['fixed acidity', 'quality', 'volatile acidity']]


## What's Next?
This mini project serves as the foundation for:
- Visualizing feature distributions
- Correlation analysis between features and wine quality
- Building predictive models for wine quality (future scope)

## Dataset
Filename: WineQT.csv

