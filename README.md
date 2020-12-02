# GIS_Project
Project repo for GIS course

## Contents
In this repository is contained two Jupyter Notebooks and three CSV files. One Notebook is the original and unorganized notebook. The other just contains the final map with its full interactive features.
The CSV files are the original unemployment data file, the file used to train the Neural Network, and the file used to generate the map.

## The Map
The map is a state level map of the United States generated using the Plotly library in Python 3. Each state has a different shade of blue based on its net forecasted change in unemployment rate over the next 6 months. There is an accompanying legend, and there are built in hover features that allow the user to see the month by month breakdown of the unemployment rate forecast for each state, along with the Root Mean Squared Error of the network for that given state that was found during testing.

## The Neural Network
The neural net used to generate these forecasts was an LSTM (Long Short Term Memory) neural net. It performed a multi-step and multi-variate time series forecast. I used much of the code found here (https://colab.research.google.com/drive/1JwDl3HZ9SfvV5crtjbuFPaU_T7Q1y34w?usp=sharing#scrollTo=ze7iac48h1JV) as a template. This code was provided in this tutorial (https://www.analyticsvidhya.com/blog/2020/10/multivariate-multi-step-time-series-forecasting-using-stacked-lstm-sequence-to-sequence-autoencoder-in-tensorflow-2-0-keras/).

## The Data
The data used for this project was directly from the Bureau of Labour Statistics in the United States. The page to download this file (and many others) can be found here (https://www.bls.gov/web/laus.supp.toc.htm). The data itself is the monthly unemployment rate by state since January 1976 until October 2020.
