2020-altitudinal-forest-vegetation-belt-model-ML

# Modelling of upwards-shifts of altitudinal forest vegetation bends due to climate change with machine-learning methods

Author: Silvana Hunger - MA Student at the University of Bern

contact: silvana.hunger@students.unibe.ch

## Introduction

The project idea is to use machine learning methods to calculate the temperatures at different vegetation belts.
This is done by using different regressor models for tests and trainsets of the different vegetation belts. The RMSE (Root Mean Square Error) describes how efficient the trained model is.

The main fuction for the models is following: 
T= f(KONT, RNORM, ETAETP, FOEHNH, GLOBRAD)

The following models are used:
 - Linear Regressor
 - Random Forest Model
 - Extra Trees Regressor
 - Decision Tree Regressor

As for the dataset, the data consist of over 80'000 measurements across Switzerland, divided in 6 vegetation belts. 
The measurements are from climate parameters and divided in January, April, July, October and Year.

## Usage

The code is provided in a Jupiter Notebook. 
For the input a unzip of the csv file samples6190.zip is necessary and the file needs to be saved in the same folder as the script.
- The csv is an excerpt from the dataset, it consists of one record for each vegetation belt.

If other input data is used, the following must be considered:
 - The attributes in the first row need to be the same
 -  The input csv name needs to be changed to the new csv 

Change of the defining test ratio
 - The test ratio can be changed from 0.2 to any number between 0 and 1, a number from 0.2 to 0.3 is recommended
 
## Results

The script calculates the RMSE for different regressor models. This is done for four month and year of each belt.
The results are saved in a csv file and can be viewed in the bar plot in Jupiter Notebook.

Following the calculation, the "Extra Trees Regressor" results in the lowest RMSE, followed by the "Random Forest Model" and the "Decision Tree Regressor". The "Linear Regressor" results are the highest.
For further calculations the use of the first two models is recommended. 

## Acknowledgement
This project was carried out within the framework of the “Geodataanalysis and Modelling” seminar at the University of Bern. 
Special thanks go to our supervisors Dr. Andreas Zischg and Dr. Pascal Horton.
