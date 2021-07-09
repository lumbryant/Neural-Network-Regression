Author: Bryant Lum

Sources:  
  https://www.sicara.ai/blog/2019-14-07-determine-network-hyper-parameters-with-bayesian-optimization
  https://www.tensorflow.org/tutorials/keras/keras_tuner  
  https://www.tensorflow.org/tutorials/keras/regression  
  https://www.tensorflow.org/tutorials/keras/overfit_and_underfit  
  https://machinelearningmastery.com/regression-tutorial-keras-deep-learning-library-python/  

The predictions are in .csv format in the main Neural Network folder. I suggest to use predictions_alldata_formatted, or predictions_toyotacovid_formatted.

The final model selected is in the ToyotaAll folder. This includes the Toyota dataset merged with all external data, 
including: Covid-19 Information, $S&P 500 Index, $CARZ Exchange Traded Fund, and Monthly Employment Level of USA.

Note: You must install TensorFlow, Keras, and KerasTuner, as well as mentioned libraries at the top of each file.

1A_mape_AllData.ipynb - Splits the training set with a 70/30 train test ratio randomly, and generates a neural network regression model, returning mae and mape.

2A_alldatapredictions.ipynb - Generates the actual predictions and should be used for future predictions. A new neural network will be generated each time, 
which is optimized to reduce loss and mape.

3A_traintest_AllData-train.ipynb - Finds train test mae and mape values.

The other folders contain the same logic with different datasets.

The R files are where the collinearity issues were checked. You do not need to run this, but may if you wish to check for collinearity issues.
