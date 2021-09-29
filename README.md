# Income Classification


<img src="https://github.com/SidhantMathur23/Income-Classification/blob/main/Income%20gifs%20and%20images/Money%20gif.gif" width="650" height="400">

## Problem Statement 
In this project, we will be implementing a use case of machine learning in the field of Personal Finances and Banking. With this data, we are tasked with predicting whether a person makes more than $50K/year.

## Project Description
#### About the Data
The dataset was taken from the 1994 census database and it consists of 32561 entries with 16 columns. The data stores various kinds of variables, 8 categorical(including the target variable) and 8 numeric variables. The target variable, labelled as "income" consists of 2 class labels, ">50K" and "<=50K". The dataset contains a class imbalance, so performany metrics like F1 score will be profoundly used as a basis to evaluate the estimator models.

<img src="https://github.com/SidhantMathur23/Income-Classification/blob/main/Income%20gifs%20and%20images/target.PNG" width="450" height="250" align="center">


#### Exploratory Data Analysis
Exploratory data analysis was performed on the dataset, which revealed some patterns in the data. Some of them being:
* The ratio of people having an income "<=50k" to ">50k" gradually decreases as we progress towards the mean, after which the ratio increases again. This means that people in lower age groups (17-35) are more likely to have incomes less than 50k than more. Similarly, people belonging to the age groups (35-60) are more likely to have incomes higher than 50k. 
<img src="https://user-images.githubusercontent.com/79369289/135263343-a99e9985-cbee-4cb6-abe9-feef1f9167ec.png" width="350" height="350" align="center">

* Dataset has a higher concentration of males than females, having a ratio of nearly 2:1. From these genders, nearly 30% of the males earn greater than 50K whereas only about 13% females enjoy an income greater than 50K. 
<img src="https://github.com/SidhantMathur23/Income-Classification/blob/main/Income%20gifs%20and%20images/gender.PNG" width="300" height="220" align="left">
<img src="https://github.com/SidhantMathur23/Income-Classification/blob/main/Income%20gifs%20and%20images/gender_dist.PNG" width="300" height="225" align="center">


Various categorical features of the dataset stored inconsistent data, specifically, the presence of "?" amongst other values. These values were replaced with np.nan values and treated using DataWig library.


## Project Setup
The project contains several external libraries which are not availible with the stndard anaconda download, these libraries are going to have be downloaded by the user. Navigate to the anaconda prompt and enter the following commands 
```python
pip install datawig
pip install category_encoders
pip install warnings
```

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.python.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://scikit-learn.org/" target="_blank"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> </a> </p>
