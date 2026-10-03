# OILMLGO-SOLUTION
Solved OILMLGO problem statement with the help of scikitlearn

# PROBLEM STATEMENT
Background----
Well logs are interpreted to estimate the petrophysical and geomechanical properties, which is essential for subsurface characterization. Various types of logs exist, and each provides distinct information about subsurface properties. Certain well logs, like gamma ray (GR), resistivity, density, and neutron logs, are considered as  conventional well logs that are run in most of the wells. Other well logs, like nuclear magnetic resonance, dielectric dispersion, elemental spectroscopy, and sometimes sonic logs, are only run in limited number of wells.
Sonic travel-time logs contain geomechanical information for subsurface characterization around the wellbore. Often, sonic logs are required to complete the well-seismic workflow or geomechanical properties prediction. When sonic logs are absent in a well or an interval, a common practice is to synthesize them based on its neighboring wells that have sonic logs. This is referred to as sonic log synthesis.




Problem Statement------

Compressional travel-time (DTC) log is not acquired in all the wells drilled in a field due to operational constraints. Under such circumstances, machine learning techniques can be used to predict DTC log to improve subsurface characterization. The goal is to develop data-driven models by processing  conventional logs from a Well  and use the data-driven models to generate synthetic compressional and shear travel-time logs (DTC respectively) in another Well. A robust data-driven model for the desired sonic-log synthesis will result in low prediction errors, which can be quantified in terms of Root Mean Squared Error(RMSE) by comparing the synthesized and the original DTC log.
You will be provided with  dataset of a Well. You need to build a model using given dataset.The model should use feature sets derived from the following seven logs: Caliper, Neutron, Gamma Ray, Deep Resistivity, Medium Resistivity, Photo-electric factor and density. The  model should synthesize two target logs: DTC log.

# SOLUTION
As this is a problem statement of regression I have used 4 regresssion models namely
1.Polynomial Regression
2.Support Vector Regression
3.Decision Tree Regression
4.Random Forest Regression
After that I have applied the training data on all these models using scikitlearn and compared the results of DTC logs from actual measurements and the results I have got after applying the models.
Decision Tree regression and Random Forest regression gave better results for training data after that I have predicted the results for test data with the help of these two models.
