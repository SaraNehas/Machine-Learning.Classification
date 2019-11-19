### Machine Learning - Classification
# Prediction of an individual year income based on its profil. 

This data was extracted from the census bureau database found at https://www.census.gov/data/tables/time-series/demo/income-poverty/cps-pinc.html
Donor: Ronny Kohavi and Barry Becker, Data Mining and Visualization, Silicon Graphics.

The prediction task is to determine whether a person makes over 50K a year.

In order to encrease the accuracy of the model, some data cleaning and data engineering has been performed on the raw data. The model generated is built with a support Vector Machine algorithm. 

So far, the accuracy score of this model with SVM algorithm is 0.86. 

Several algotithms were tested (Logistic Regression, K-Neighbors Classifier, etc) but have lower accuracy scores.

Here below is a description of the fnlwgt (final weight) data/column.

The weights on the CPS files are controlled to independent estimates of the civilian non-institutional population of the US by Population Division. These are:
   1.  A single cell estimate of the population 16+ for each state.
   2.  Controls for Hispanic Origin by age and sex.
   3.  Controls by Race, age and sex.

 The census bureau uses all three sets of controls in their weighting program and "rake" through them 6 times so that by the end they come back to all the controls they used.
 
 The term estimate refers to population totals derived from CPS by creating "weighted tallies" of any specified socio-economic characteristics of the population. People with similar demographic characteristics should have similar weights.  There is one important caveat to remember about this statement.  That is that since the CPS sample is actually a collection of 51 state samples, each with its own probability of selection, the statement only applies within state.
