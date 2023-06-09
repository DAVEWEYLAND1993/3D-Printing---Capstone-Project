# Bayesian Optimisation of 3D Printer Dataset for Mechanical Engineers


## NON-TECHNICAL EXPLANATION OF YOUR PROJECT

The purpose of this notebook was to implement a so-called Trust Region Bayesian optimisation algorithm for identifying ideal input parameter adjustments for 3D printing and compare its performance against Grid Search, Random Search and HyperOpt Bayesian Optimisation. The input parameters have a huge impact on 3D print quality, accuracy and material strength, therefore identification of optimal combinations of such parameters is of paramount importance to researchers and engineers. The Trust Region Bayesian Optimisation (TurBO) algorithm (invented by Uber) is algorithm that specialises in high-dimensional problems and could theoretically yield better results than other commonly used algorithms.

## DATA

Data was compiled by a research team of TR/Selcuk University's Department of Mechanical Engineering. Dataset is available to the public free of charge on Kaggle: https://www.kaggle.com/datasets/afumetto/3dprinter?resource=download&select=data.csv

Code for modelling was obtained from GitHub - https://github.com/MBKraus/Hyperopt/blob/master/Hyperopt.ipynb and BoTorch website- https://botorch.org/tutorials/turbo_1
 
## MODEL 

I used Random Search, Grid Search, HyperOpt (with LGBMRegressor) and TurBO Bayesian optimisation models to see if there was any siginificant difference in output and performance. 

## HYPERPARAMETER OPTIMSATION

Hyperparameters that were optimised: Learning Rate, Maximum Depth, Number of Leaves, Number of EStimators, Boosting Type, Column Sample by Tree, Lambda Regularisation, Adam Optimisier etc.

## RESULTS
 
Better performance by TurBO was expected



