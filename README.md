<h1 align="center">Ethereum Phishing Detection using Ensemble of Classical and Quantum Machine Learning</h1>

This project aims to develop a comprehensive framework for phishing detection that can effectively analyze transaction data, identify potential phishing attempts, and provide real-time alerts to users. By enhancing the security of Ethereum
transactions, this approach aims to mitigate the risks associated with phishing attacks, protect user assets, and promote trust within the Ethereum community.

## Methodology:
The model is built by taking a QSVM model and an LGBM model as base classifiers and then two-way stacking a Logistic Regression model on top. We train the base
classifiers QSVM and LGBM using 320 training data points, then we predict the labels of both training data and testing data using the trained classifiers.
The labels we obtained are added as features to initial training and testing data sets, thus our final training data and testing data with appended features consists of total 9 features(one label is added from each classifier). The logistic regressor model (meta classifier) is trained using the appended training data and the corresponding labels.

## LGBM
