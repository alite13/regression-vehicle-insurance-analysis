# Regression-Vehicle-Insurance-Analysis  
This is the course project for the CAP 5610 - Machine Learning course at the University of Central Florida, Fall 2022.  
This is the repository for the source code of the prediction of the vehicle insurance claim amounts using statistical and machine learning methods. We compare several linear regression models to generalized linear models when modeling the pure premium of insurance claims. We explore linear regression algorithms such as the Tweedie GLM Regressor, Decision Tree, Random Forest, K-Nearest Neighbors, Support Vector Machine, Adaptive Boosting with Decision Tree Regressor as base estimator, and Sequential Neural Network. We benchmarked these with a compound Poisson-Gammma Generalized Linear Model which is what's commonly used in actuarial data science.  
We explore these methods on a French motor third-party liability insurance dataset.  
## Datasets can be found here:

[Dataset containing claim amounts for 26639 third-party liability policies](https://www.openml.org/d/41215)  

[Dataset containing risk features for 678013 motor third-party liability policies (observed mostly on one year)](https://www.openml.org/d/41214)  

In the two datasets, risk features are collected for 678013 motor third-party liability policies (observed mostly on one year), in addition to claim numbers by policy as well as their corresponding claim amounts. freMTPL2freq contains the risk features and claim counts, while freMTPL2sev contains claim amounts. Both tables can be linked together via the corresponding policy ID.  

Insurance companies are usually interested in predicting claim frequency, claim severity, pure premium, and/or loss ratio for each policyholder in their portfolio.  

In this notebook, we are predicting the **Pure Premium: Claim Amount / Exposure**.  

Definitions:  

**Claim severity**: Claim amount per claim or occurrence  

**Pure premium**: Claim amount per exposure  

**Loss ratio**: Claim amount per premium amount  

**Claim frequency**: Claims per exposure  

**Policy**: contract between the insurance company and the policyholder  

**Claim**: request filed by a policyholder to the insurer provider for compensation for a covered loss  

**Claim amount**: amount of money the insurance pays to the policyholder  

**Exposure**: the duration of the insurance coverage of a given policy, in years  

 
## Dependencies (Anaconda):  

Scikit-learn 1.1.0 (`conda install -c conda-forge scikit-learn`)  

Scipy 1.8.1 (`conda install -c conda-forge scipy`)  

Numpy 1.23.1 (`conda install -c conda-forge numpy`)  

Matplotlib 3.5.2 (`conda install -c conda-forge matplotlib`)  

Seaborn 0.11.2 (`conda install -c conda-forge seaborn`)  

Pandas 1.4.3 (`conda install -c conda-forge pandas`)   

Tensorflow 2.3.0 (`conda install -c conda-forge tensorflow`)  

Keras 2.4.3 (`conda install -c conda-forge keras`)   

This project is implemented using Python 3.8.5.
