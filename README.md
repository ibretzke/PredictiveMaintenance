# PredictiveMaintenance
Predictive maintenance of aircraft turbine

The example based on the simulated test data and template from Azure AI Gallery(https://gallery.azure.ai/Experiment/Predictive-Maintenance-Step-2A-of-3-train-and-evaluate-regression-models-2).
This template uses the example of simulated aircraft engine run-to-failure events to demonstrate the predictive maintenance modeling process.

There are two modelling solution which are realized with help of LSTM neural network:

- Regression: Predict the Remaining Useful Life (RUL), or Time to Failure (TTF)
- Binary classification: Predict if an asset will fail within certain time frame(in this case cycles).

There are three datasets as inputs. 
- Training data: It is the aircraft engine run-to-failure data (PM_train.txt).
- Testing data: It is the aircraft engine operating data without failure events recorded (PM_test.txt).
- Ground truth data: It contains the information of true remaining cycles for each engine in the testing data (PM_truth.txt).

The last cycle in each time series (all elements with the same id) can be considered as the failure point of the corresponding engine.
