
# IRIS DATA SET
## Exploration of the Iris Data set using Python

## Main Python files in this repository

- IrisData_mean.py: An initial attempt to write simple functions on irisdata set as csv file
- IrisData.py: A basic few lines of code to import csv file and sort into rows and column
- IrisData_split: Displays a script researched on Stackoverflow to split dataset using basic python code
- IrisData_np.py: Contains simple function to determine means of all species
- IrisData_np_v2.py Main Python file worked on. Attempt to import pandas, numpy and matplotlib packages and work on data set,
-  Sorting data into species and characteristic
- Output means of each characteristic for each species
- Overall summary of entire iris data: count, mean sd, min, %, max
- Output and label simple line graphs
- Output and Label Histograms
- Iris.seaborn.py: A brief investigation into the usefulness of the Seaborn package for data visualisation on the Iris set

# 1.0 INTRODUCTION

### 1.1 The Iris Data Set

The iris data set was first described in a paper written by R.A. Fisher in the Annals of Human Genetics in 1936. It is a data set of 50 samples which the author gathered on each of three species of Irises: setosa, versicolor and virginica. Measurements of 4 properties of 50 flowers of each of the plants were taken, namely Sepal length, Sepal width, Petal Length, and Petal width. The author suggests that the petal and sepal lengths and widths are characteristics whcih can be used to identify which species they belong to based on a linear discriminant model. Fischer himself developed the linear discriminant model,a statistical, machine learning and pattern recognition technique used to distinguish between two or more objects, classes or events.

### 1.2 Simple Python functions

A simple function to calculate the mean of a column is seen here in irisdata.
Using the Numpy package has the 'mean' function built in so it can be seen in further work that writing a function to define the mean is not really necessary.

### 1.3 Python Libraries

### Pandas
The pandas library is a useful package for importing labelled data such as the iris data set. It makes data such as csv files much easier to work with.

### Numpy

The NumPy package is a basic package for scientific computation in python. It is also particularly useful as a container for multidimensional data which makes NumPy arrays easy to work with,manipulate and analyse. This allows NumPy to seamlessly and speedily integrate with a wide variety of databases.
defines CSV files as >"Comma separated values text files (.csv), in which the comma character (,) typically separates each field of text." CSV files are difficult to work with since the commas and other strings must be removed and the float and/or integer data must be then sorted and worked on. Numpy was found to be particularly useful for importing the data set as an array (matrix) or 'list of lists' on which various functions could be applied. Attempts were made in the IrisData_split.py file to write code which allowed the data set to be split without using the Numpy package.

### Matplotlib

The Matplotlib python library is used to make charts such as histograms, plots and bar charts. The pyplot module is used in this project to generate simple histograms of the python data set for example in file 'Iris_data_np_v2.py'. Addition of add-on toolkits such as 3d plotting with mplot3d enhance the functionality of the matplotlib library.

### Scikitlearn

Scikitlearn is a useful library for carrying out machine learning in python and contains many machine learning models which may be used to explore data sets. Scikitlearn already has built in code to handle the machine learning analysis of large data sets.

### Seaborn package

Seaborn is a Python visualization library based on matplotlib. It provides a high-level interface for drawing attractive statistical graphics.

## 2.0 EXPERIMENTAL
#### 2.1 Downloading and importing the Data Set

The file iris.csv in this repository contains the csv data for the iris data set. This was accessed from the UCI machine learning repository located.

#### 2.2 Plots and histograms of the Iris Data set

Plots and histograms of the Iris data set was carried out by first separating out the rows and columns of the data set into species and characteristic. Use of the data import, analysis and display properties of pandas, NumPy and Matplotlib respectively were used through trial and error to find the appropriate commands.

Using the seaborn package, plots (scatterplot matrices) were generated showing the relationship between attributes for each species.

#### 2.3 Simple Statistical Analysis

Simple calculations on the data set might involve getting the mean of each column i.e. looping through column 1 to 4, getting the sum of each column and dividing by the number of rows to get the mean. This loop would have to terminate at the strings in the data set. The file IrisData_mean.py uses pandas to import the csv file which is then converted to a Numpy array using the NumPy package. The file is then split easily by species and characteristic. Means are calculated for each characteristic; Sepal length, Sepal width, Petal Length,and Petal width for each species to three decimal places.

#### 2.4 Machine Learning

Machine learning may be defined as 'creating and using models that are learned from data' Typically the goal of machine learning is to take a data set whose relationships we understand (a training set), use it to develop models which are then used to predict various outcomes for new, data. A 'model' may be defined as "The specification of a mathematical (or probabilistic) relationship that exists between different vasriables".

In the case of the Iris Data set investigated in this project the goal of a machine learning algorithm might be to predict the species of iris based on an unknown set of petal and sepal width and lengths (or even just the data from one measurement such as petal length.)

#### 2.4.1 Models

 Different types of machine learning models exist including

- Supervised Where the (training) data is labelled with the right answers: e.g. Classification or regression
- Unsupervised Where the data set has no labels: e.g. Clustering
- semisupervised some data are labelled
- Online Where the model has to adapt continuously to new data

#### 2.4.2 Machine Learning carried out on Iris Data Set

The Scikitlearn library site contains various examples of machine learning models of the Iris data set including principal component analysis, logistic regression and nearest neighbours classification (amongst others) 

### 3.0 DISCUSSION AND CONCLUSION

The Iris Data set contains a relatively simple number of measurements which can be elegantly used to statistically differentiate different data sets and use those data sets to develop mechine learning algorithms to predict and classify unknowns.

Initial attempts to import the csv file and split it using basic python code proved cumbersome. The Pandas library simplified the process of data import and manipulation as seen in the Iris_final_Pjt.py script and in subsequent work.
