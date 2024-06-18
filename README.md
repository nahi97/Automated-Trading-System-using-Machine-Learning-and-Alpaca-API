## Automated Trading System using Machine Learning and Alpaca API
## Project Overview
This project aims to apply machine learning techniques to financial market datasets to develop models that enable better, automated trading decisions. The system fetches real-time market data, processes it using a machine learning model, and executes trades based on model predictions. The project uses Python and integrates with the Alpaca API for real-time trading.


### Features
<li>Fetch historical and real-time market data using the Alpaca API</li>
<li>Develop and train machine learning models to predict stock prices</li>
<li>Execute trades based on model predictions</li>
<li>Backtest trading strategies</li>
<li>Schedule tasks to automate trading</li>

### Requirements
<li>Python 3.8 or higher</li>
<li>Alpaca API Account (free or paid)</li>

### Installation
<li>Clone the repository</li>

<li>Install required packages</li>

<li>Set up your Alpaca API credentials</li>
<li>Create a .env file in the root directory and add your Alpaca API credentials</li>

<li>Run the Model Training Script</li>

<li>Run the Real-time Trading Script</li>


### Model Development
<li>Data Collection and Preprocessing: Historical data is fetched using the Alpaca API and preprocessed to handle missing values, normalize/standardize features, and create additional features like moving averages and volatility. </li>
<li>Model Training: A Random Forest Regressor model is trained using the preprocessed data. The model's hyperparameters are tuned using GridSearchCV to achieve optimal performance.</li>
<li>Evaluation: The model is evaluated using Mean Squared Error (MSE) and other relevant metrics. The best model is saved for real-time trading.</li>

### Trading Strategy
  <li>The trading strategy is based on the predictions made by the machine learning model.</li>
  <li>Buy signals are generated if the predicted price is higher than the current price.</li>
  <li>Sell signals are generated if the predicted price is lower than or equal to the current price.</li>

### Backtesting
<li>The backtesting script evaluates the trading strategy on historical data to assess its performance.</li>
<li>Key performance metrics such as Sharpe Ratio and Maximum Drawdown are calculated.</li>

### Real-time Integration
    
The real-time trading script fetches the latest market data, makes predictions using the trained model, and executes trades based on the predictions.

### Scheduling Tasks
The schedule module is used to automate the execution of tasks at regular intervals, such as fetching data, making predictions, and placing trades.

