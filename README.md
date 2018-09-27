#Heartsteps version two


Each directory contains code for doing a certain task. We also have a lookup table at the bottom of this page which tells you where to find the code of a certain person. 


The [data processing(/data_processing) folder contains all of the code for processing the raw data. The difference between this directory and analysis, is that these scripts take raw data and output data in another form. For example, here we might have a script which takes all of the raw sensor readings and produces a time series with no missing values. On the other hand, in analysis, we might have a script that takes the time series with no missing values and calculates the average number of sedentary periods throughout the population. 
 
 
The [models(/models) folder contains all of the code for running models. The difference between a model and analysis might be fuzzy. Here, we will make this distinction. Any time you have a model which has parameters which need to be learned, and outputs some values y, given input x, conditioned on parameters, this should go in this folder. If you take the output of a model, or if you take the output of a data processing script, and produce a statistic, or answer some question about the data this is not a model. A model is an object which can produce data, given input and parameters. 

