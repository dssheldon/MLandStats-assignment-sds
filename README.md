# Exploring the Scikit-Learn and SciPy Stats



<img src= "https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg"   alt="Scikit logo" style="float: center; margin-right:10px;" width="200" height="70" />  <img src= "https://upload.wikimedia.org/wikipedia/en/5/58/Scipylogo.png"   alt="SciPy logo" style="float: center; margin-right:10px;" width="200" height="50"/>



<b>Prepared by:</b>  Sheldon D'Souza
<b>Student Number:</b>  G00387857
<b>Module:</b>  Machine Learning and Statistics, Winter 21/22

***

## Objective of the Repository
The objective of this repository is to to explore the Scikit-Learn and SciPy Stats libraries and show the functionality of these repositories through the use of appropriate datasets.

This repository contains Jupyter notebooks and other relevant files to complete this objective for the module “Machine Learning and Statistics, Winter 21/22”.


## Contents of the repository

The contents of this repository are as follows:

1. .gitignore
2. LICENCE
3. Readme.md (this file)
4. requirements.txt (library requirements to run the workbooks)
4. scikit-learn.ipynb
5. scipy-stats.ipynb
6. diabetes.csv (within the 'files' folder)
7. stcp-Rdataset-Diet.csv (within the 'files' folder)
8. iris.csv  (within the 'files' folder)

The diabetes.csv file contains the dataset which will be used to explore the sci-kit learn library
The stcp-Rdataset-Diet.csv will be used to perform the one-way ANOVA using scipy stats


## Installation

##### Steps to Install necessary pacakges

1.  Install `python` 
2. Install `jupyter` by typing ```pip3 install jupyter``` in the command line
3. install the necessary packages from requirements.txt using ```pip install -r requirements.txt```
4. Alternatively, you will need the following packages:
	- matplotlib==3.3.4
	- numpy==1.20.1
	- pandas==1.2.4
	- scikit_learn==1.0.2
	- scipy==1.6.2
	- seaborn==0.11.1      

The most efficient way to do the above  is to install the `anaconda` package from: [Anaconda.com](https://www.anaconda.com/)


## Quick Run

You can view the notebooks in static form (`nbviewer`) and dynamic form (`binder`) by clicking the following badges:

<i>Scikit-learn Workbook:</i>
[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/dssheldon/MLandStats-assignment-sds/blob/main/scikit-learn.ipynb)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dssheldon/MLandStats-assignment-sds/HEAD?labpath=scikit-learn.ipynb)



<i>Scipy-stats Workbook:</i>
[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/dssheldon/MLandStats-assignment-sds/blob/main/scipy-stats.ipynb)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dssheldon/MLandStats-assignment-sds/HEAD?labpath=scipy-stats.ipynb)

## Run

To run the workbooks, you will need to perform the following steps:

1.   Open command terminal (`cmd` in windows)
2.   Navigate to the folder where the notebook is from within the terminal
3.   enter `jupyter notebook` or `jupyter lab` at the command line 
4.   your browser should automatically open with `jupyter notebook` running
5.   select the notebook you want to navigate and commence viewing or editing


## Exploring the notebooks

##### Exploring Sci-kit Learn
This will be done within  the  Jupyter notebook named scikit-learn.ipynb. 
The notebook commences with  a brief overview of the scikit-learn library including it's use, advantages and disadvantages.
The notebook then contains an analysis of the Pima Indians Diabetes Database and aims to predict the onset of diabetes based on diagnostic measures. The notebook also contains an analysis of the classic iris dataset and aims to predict one of the fields of by reference to other fields within the dataset.
Key steps within this notebook contain:
- importing the dataset and converting it into a `pandas` dataframe
- exploring the dataset through the `info` and `describe` functions in `pandas`. Also looking to see whether there are any NaN or nil values within the dataset
- cleaning the dataset by dropping unnecessary columns (based on the exploration above) and substituting nil values with relevant data
- performing various analysis on the dataset including `pairplots`, `heatmaps` and `boxplots` using the `seaborn` and `matplotlib` packages
- using the scikit-learn library to import and perform various machine learning algorithms to make predictions including tweaking parameters within these algorithms
- compare the algorithms to see which is the most effective

##### Exploring SciPy Stats
This will be done within  the  Jupyter notebook named scipy-stats.ipynb
The notebook commences with  a brief overview of the scipy and the scipy stats  library including it's use and description of it's relevant functions.
The notebook then contains a one way ANOVA  of a diet dataset.  data set contains information on people who undertook one of three diets. There is background information such as age, gender, and height. The aim of the study was to see which diet was best for losing weight.
Key steps within this notebook contain:
- importing the dataset and converting it into a `pandas` dataframe
- exploring the dataset through the `info` and `describe` functions in `pandas`. Also looking to see whether there are any NaN or nil values within the dataset
- cleaning the dataset by dropping unnecessary columns and substituting nil values with relevant data
- analyzing  whether the six assumptions on the dataset for performing ANOVA are fulfilled including using plots to perform this analysis 
- using the scipy stats package perform one-way ANOVA on the dataset and analyse the results
- perform a simple post-hoc test and interpret results


##### Intersting things to try in the notebooks:

Look analysis performed within the workbooks and the observations and conclusion on these analysis. 

scikit-learn.ipynb: the parameters used in the models can be modified to change the efficacy of the models used and the results thereof.

scikit-learn.ipynb: for the iris dataset, the user can modify the number of independent variable or can swap the dependent variable for an independent variable to see the impact on the efficacy of the model used.

scipy-stats.ipynb: remove the single outlier from the dataset and check the impact on the ANOVA.

scipy-stats.ipynb: consider using a two way ANOVA to check whether sex of the participant along with the diet had an impact on weight loss

Tweak the parameters of the plots within the workbooks. As an example 
1. size of the plots can be changed by changing the ```plt.rcParams["figure.figsize"]``` parameters before the plots are rendered
2. scikit-learn.ipynb: the number of boxplots can be changed by tweaking the ```fig, axs = plt.subplots(ncols=4)``` parameter.

Change the `randomstate` variable within the workbooks to produce reproduceable results (see limitations below)


## Troubleshooting
1. If the workbooks do not render correctly: check that you have followed the installation and run instruction above
2. If your browser does not automatically open the jupyter lab from the command line: clear the cache (shift + refresh) and close and open the browser again

 ## Limitations:

As the Notebook uses the random sampling functions  within Scikit-Learn and Pandas, the 'random_state' argument has been used to ensure that the training and testing data remains consistent in the Notebook. The random_state variable should be set to 'None' within the import module cells of the notebook if the user requires the training and testing data to vary with each running of the workbook. 

## Contact

[Sheldon D'Souza](g00387857@gmit.ie)