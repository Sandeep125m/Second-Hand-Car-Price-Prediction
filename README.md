# Second-Hand-Car-Price-Prediction
This project aims to predict the resale price of second-hand cars using a supervised machine learning approach, specifically leveraging deep learning with TensorFlow and Keras.


Project Overview
----------------
- Predicts prices of second-hand cars using machine learning.
- Built using TensorFlow and Keras Sequential API.
- Based on structured data (CSV file).

Data Summary
------------
- Source File: train.csv
- Features Used:
  * years, km, rating, condition, economy, top speed, hp, torque
- Target Variable: current price

Data Preprocessing
------------------
- Dataset loaded using pandas.
- Converted to TensorFlow tensor.
- Normalized using tf.keras.layers.Normalization.
- Split into Train (80%), Validation (10%), and Test (10%).

Model Architecture (Sequential API)
-----------------------------------
- InputLayer for 8 features
- Normalization layer
- Dense(128, activation='relu') x 3 layers
- Final Dense(1) output layer

Compilation & Training
----------------------
- Optimizer: Adam (learning_rate=0.1)
- Loss: MeanAbsoluteError
- Metric: RootMeanSquaredError
- Trained for 100 epochs

Visualizations
--------------
- Pair plots for feature correlation
- Line plots of loss and RMSE over epochs
- Bar chart for predicted vs actual prices

Evaluation
----------
- model.evaluate(X_val, y_val) for validation
- model.evaluate(X_test, y_test) for testing
- model.predict used for forecast
- Results shown for 100 examples

Notebook Statistics
-------------------
- Total Cells: 46
- Code Cells: 43
- Markdown Cells: 3
