# Write-a-Data-Science-Blog-Post

## Installation

- Libraries used for this application are:
- re, sys, os, datetime
- matplotlib.pyplot
- numpy as np
- pandas as pd
- sklearn.linear_model - LogisticRegression
- sklearn.model_selection - train_test_split
- sklearn.metrics - accuracy_score

## Business Understanding

Health data is used much more frequently today in analysing workout performances to support training plans and health monitoring. Health apps and data is particularly focussed around heart rate measurements which gives the user indicators of physical fitness levels and spikes or health warnings.

This article takes a deeper look into heart rate data and highlights the variables which affects the accuracy in being able to predict heart rate performance based on elevation. To address this we posed the following questions:

- What is the stability of heart rate measurements from Apple watch device?

o When using the workout app, typically how many heart rate measurements are taken per workout?

o On average, how long does it take to register the first heart rate measurement above 130 bpm?

- How much does elevation have an effect on heart rate performance during running?

- Can this information be used to predict heart rate during a running activity?

## Data Understanding

1) AppleHealthData.csv (this file is stored on this repository as a zip). This is initially exported from Apple health. This data contains multiple health entries such as heart rate. This information is explored in file "Workout Data Performance.ipynb"
2) combined_gpxdata.csv - This is a combination of multiple .gpx files which has been combined from Apple health export. This data contains workout information by tracking date/time, elevation and latitude and longitude which has been removed from this file for sesnsitivity. 

## Prepare Data

The data used is a relatively high quality. Data preparation is. Carried out in the file "Workout Data Performance.ipynb"  which drops data not required and handles categories values for modelling.

## Data Modelling

Data modelling techniques in this project is using logistic regression. 

## Evaluate the Results

Results can be found in the following Medium post - https://medium.com/@hinton_/ai-model-accuracy-at-predicting-workout-heart-rate-4bd22d38d845
