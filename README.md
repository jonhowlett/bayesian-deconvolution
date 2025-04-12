This repository contains Stan code for Bayesian hierarchical regression for fMRI data and Bayesian deconvolution to estimate individual cognitive parameters based on BOLD signal.

All scripts take a single BOLD signal timeseries (e.g., extracted from an ROI and possibly residualized to control for nuisance regressors prior to the Bayesian analysis).

Bayesian_hierarchical_regression_BOLD.stan performs Bayesian hierarchical regression with a set of arbitrary regressors at the trial level. 
It convolves regressors with the hemodynamic response function (HRF) and estimates individual-level and group-level coefficients for each regressor.

MID_individual_learning_rate_model.stan implements a learning model based on Rescorla Wagner (RW) for the monetary incentive delay (MID) task. 
It estimates individual learning rate parameters in incentive learning (i.e. prediction of the absolute value of the incentive cue), e.g. in the striatum.

MID_individual_persistent_prior_model.stan implements a learning model based on Rescorla Wagner (RW) for the monetary incentive delay (MID) task. 
It estimates individual persistent prior parameters in incentive learning (i.e. prediction of the absolute value of the incentive cue), e.g. in the striatum.
