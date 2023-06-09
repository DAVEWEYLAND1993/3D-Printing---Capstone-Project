# Model Card


## Model Description

**Input: 3D Printer Setting Parameters (Layer Height/mm, Wall Thickness/mm, Infill Density/%, Infill Pattern, Nozzle Temperature/C, Bed Temperature/C, Print Speed/mm per sec, Material, Fan Speed/%)**

**Output: Roughness/micrometer, Tension (ultimate) Strength/MPa, Elongation/%** 

**Model Architecture: Random Search, Grid Search, HyperOpt (Bayesian Optimisation) - code adapted from MBKraus - https://github.com/MBKraus/Hyperopt/blob/master/Hyperopt.ipynb  and TurBO Bayesian Optimisation - code adapted from https://botorch.org/tutorials/turbo_1**

## Performance

Performance was to be evaluated by various matrics (e.g.: cross-validation socre, time elapsed etc.). For Randon, Grid, HyperOpt search I made use of an LGBMRegressor.

## Limitations

Coming up with surrogate functions was a very difficult task for a multi-dimensional problem such as this. Information available on correlations between input parameters is scarce. Technical issues with code implementations were also present. Furthermore, this was not a particularly large dataset, so it would not be possible at this point to draw any meaningful conclusions.

## Trade-offs

Hyperparameter tuning (altering arguments) had major effect on performance
