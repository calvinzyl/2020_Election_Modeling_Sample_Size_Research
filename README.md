# 2020 Election Modeling & Sample Size Research

## Overview

This repository is a companion to the Fall 2022 QMSS capstone course at Columbia University, in collaboration with Bluelabs, a leading provider of data science services and products for presidential politics. This project explores the propensity to vote for party candidates by producing models with
demographically representative survey data. These data include 45,027 responses from voters across numerous demographic groups in the 2020 election cycle. The complete analysis is split into three modeling groups: presidential model (split by registered & non-registered states), senate model (Kentucky), and gubernatorial model (Virginia). I myself was specifically responsible for the gubernatorial modeling, so you will only find the raw codes for the governor models and validation results.

In this repository, you will find three files: **final presentation**, **white paper**, and **governor models**, documenting our codes, outputs of modeling and analysis, and formal deliverable.

## Project Roadmap
- **Support Models: Logistic Regression** <br>
The support models provide predicted probabilities (rather than linear coefficients) for each of our binary dependent variables. These models provide coefficients that are easily communicated, scored, and compared. For each modeling team, we began the initial process of cleaning data by removing unnecessary data. We also imputed median and means for any missing values, recoded categorical variables, and removed others to address issues of multicollinearity. After the initial cleaning, each team began the process of feature selection using supervised L1 regression models to identify significant features. Upon manual review and adjustment, we imputed these features into Logistic Support Models to form predictions on training, testing, and full data separately. Lastly, each team retrieved the feature coefficients for each variable for future usage.<br>
- **Validation: Cross-tabulating Sociodemographic Groups & Decile Graphs**<br> 
We utilized the coefficients retrieved from the previous step to compare the differences between the true average values grouped by demographic variables and the predicted values grouped by demographic variables.<br>
- **Sample Size Research: Monte-Carlo Simulation** <br>
Once an acceptable degree of efficacy was reached for each of our models, we began to explore variations in accuracy rates for different sample sizes. We elected to use a Monte Carlo Simulation method. Monte Carlo Analysis allowed us to predict the accuracy for a variety of sample sizes. Thus, by simulating different levels of sample sizes and running the data over the logistic model, we are able to identify the most suitable sample size to be used for our analysis.<br>

