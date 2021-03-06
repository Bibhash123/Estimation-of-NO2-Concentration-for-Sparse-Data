# Estimation-of-NO2-Concentration-for-Sparse-Data
This repository consists of the code implementation for the paper titled "Estimating Near-Surface Nitrogen DioxideConcentration From Sparse Satellite Dataset". The work deals with the estimation of near-surface concentration of Nitrogen Dioxide over an area above southern europe using satellite measured tropospheric vertical column density values.

For the mitigation of the threat of pollution, round-the-clock measurement of atmospheric pollutants is imperative.Nitrogen Dioxide (NO2) is one of the major atmospheric pollu-tants, having adverse effect on human health. Traditionally,insitumeasurement strategies have been used for monitoring NO2concentrations, thus limiting the study only to urban locationswhere monitoring stations are available. Satellite monitoringoffers a truly global alternative. In recent years various methodshave been proposed for estimation of near-surface concentrationsusing tropospheric vertical column densities. These methodsuse a number of other variables such as weather parameters,demographic attributes, and geographic parameters. In this workwe study the performance of a Convolutional Neural Networkfor the task in an univariate scenario, i.e with only troposphericVCD as the regressor, It is found that when the data is sparse innature, the CNN shows a RMSE score of 14.692μg/m3, and isoutperformed by methods such as Linear Regression, XGBoostand LightGBM. However, as the sparsity in data reduces, CNNperforms better than the other methods considered for the study.

![image](https://user-images.githubusercontent.com/64698873/144715750-3969a6bd-6eb9-4655-ae76-04a8ce801541.png)

The above image compares the predicted cocncetration patterns of different models such as Linear Regresssion, LightGBM and XGBoost against that of convolutional neural networks.
The dataset used for the study can be accessed at : https://www.kaggle.com/bibhash123/grsldata


## Files In the Repository
<pre>
./
+-- README.md
|+--- <b>Model Training</b>
|    +----------- <i>GRSL_Model_Training.ipynb</i>: Training of convolutional neural network for the dataset
|+--- <b>Data-Preparation</b>
|    +----------- <i>Data_Preparation_GRSL.ipynb</i>: Pipeline to perform the gridding procedure for the dataset
|+--- <b>Benchmarking</b>
|    +----------- <i>GRSL_Benchmarking.ipynb</i>: Benchmarking of convolutional neural network against linear regression, xgboost and lgbm.

</pre>
