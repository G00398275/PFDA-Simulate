# Programming for Data Analysis 2021 - Project
***

# Simulating a real world problem

## Author: Ross Downey (G00398275)

## Programming for Data Analysis 2021: Galway Mayo Institute of Technology

## Lecturer: Dr. Brian McGinley
***

![](https://github.com/G00398275/PFDA-Simulate/blob/main/images/horse_finish_line.png?raw=true) 

For this project I will be creating a dataset to simulate a real-world problem. In this case I will be simulating data based on a famous horse race, the Aintree Grand National. The simulations will be based on previous historical trends in this race, and a statistical model will be created based on previous performance characteristics of successful horses (Age, Weight, Rating, Odds, etc.)  Some of these variables are related, and some are independent of each other. With the aid of python code and plots I will build a simulation to help predict likely winning participants in the race.
The simulation is located in the Jupyter notebook "Simulate.ipynb" contained in this folder.

## Install
***


These are the steps to install the required software packages to run the notebook:

1. Download [Anaconda](https://www.anaconda.com/),
 or should the entire Anaconda package not be required download [Python](https://www.python.org/downloads/)
2. Download [CMDER](https://cmder.net/) or other suitable console terminal.


## Run
***

This is how to run the notebook

1. Open console terminal
2. Enter 'jupyter lab'
Note: Jupyter lab is run on your default internet browser. 

Alternatively, the following badges can be clicked to run the notebook:

NB Viewer for a static version of the notebook  

[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://github.com/G00398275/PFDA-Simulate/blob/main/Simulate.ipynb)  


Binder for a dynamic copy which you can edit if required  

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/G00398275/PFDA-Simulate/HEAD?labpath=Simulate.ipynb)

## Explore
***

Have a look at the jupyter notebook 'Simulate.ipynb'. As mentioned previously it simulates runnings of the famous Aintree Grand National horse race. Simulations have been created based on the statistics of previous winners. The statistics considered were age, weight, breeding, odds, and rating. Based on the the trends of winners of this race from the previous twenty years I have simulated two hundred runnings of the race added all data to a dataframe. This dataframe provides a guideline as to the probable characteristics of a winning horse in this race. This could be used to help predict successful horses in this steeplechase.  

As certain assumptions are made when building this simulation, and some outliers have been removed based on this author's opinion, adjustments can be made to this notebook if required on a user's copy. Also, in subsequent years trends may change, e.g. the age profile of winners could change based on rule changes in the race. Should the user wish to change a simulated variable it can be done as follows:

` rng = np.random.default_rng()   

age = rng.integers(low=8, high=12, size=200)  
age`  


This is the code used to generate the age of winning horses in a uniform distribution. If the age profile changes then the user can adjust the low or high values. If the user wishes to simulate more than 200 races, then they can increase the size values. If the distribution type is required to be changed then a different type of numpy distribution is required. See [numpy](https://numpy.org/doc/stable/user/) for further information on distribution types.

## Credits
***

I used a number of different packages in this jupyter notebook to help simultate data (numpy) and plot data (matplotlib, seaborn) etc. 
Details of the packages used are included below:

### Numpy

Numpy, or numerical Python, is a library used in Python to create different types of arrays or multi-dimensional matrices, and includes a large collection of mathematical functions to operate on these arrays.[1]. In this case Numpy will be used to simulate data using the numpy.random package based on certain mathematical distributions.  

### Pandas
 
Pandas is an open source library built for data analysis and manipulation in Python

### Matplotlib
  
Matplotlib is a plotting library used in python to create visual plots from data. For this case Matplotlib will be used to create certain plots to help present large amounts of numerical data, generated using Numpy, in a clear and concise manner using histograms, charts etc.  

### Seaborn  
 
Seaborn is also a plotting library used in Python. It is based on Matplotlib, but in this author's opinion can yield more visually appealing plots than Matplotlib in certain cases.  

### SQLite 3  

SQLite 3 is used to create an embedded database, this can be used to edit the simulated database when required.  


