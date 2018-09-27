#Heartsteps version two


Each directory contains code for doing a certain task. We also have a lookup table at the bottom of this page which tells you where to find the code of a certain person. 


The [data processing](/data_processing) folder contains all of the code for processing the raw data. The difference between this directory and analysis, is that these scripts take raw data and output data in another form. For example, here we might have a script which takes all of the raw sensor readings and produces a time series with no missing values. On the other hand, in analysis, we might have a script that takes the time series with no missing values and calculates the average number of sedentary periods throughout the population. 
 
 
The [models](/models) folder contains all of the code for running models. The difference between a model and analysis might be fuzzy. Here, we will make this distinction. Any time you have a model which has parameters which need to be learned, and outputs some values y, given input x, conditioned on parameters, this should go in this folder. If you take the output of a model, or if you take the output of a data processing script, and produce a statistic, or answer some question about the data this is not a model. A model is an object which can produce data, given input and parameters. 


 
The [analysis](/analysis) folder contains all of the code for performing analysis. This is a broad category. Basically, if something takes some processed data and computes some information about it, that is analysis. For example, you might take the output of a model, and look at its characteristics. Or you might take some data that has been processed, and compute its characteristics. For example, if you are looking at the average user step counts, or the weather patterns, that might go in the analysis folder. This might be different than evaluation. 

The [evaluation](/evaluation) folder contains all of the code for performing evaluation. What differentiates evaluation from analysis? If there is no distinction for you, just put it in analysis. Basically, evaluation tells you how well a model does something. If a model takes input and gives you output, you want to know how well this generated output matches your ground truth output. This tells you something about the model. 


The [other](/other) folder is for everything that you can't categorize. Try to categorize, this is a last resort. 