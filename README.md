
# Stock Price Prediction

This project uses two different models for comparison, the Facebook Prophet model and a Long Short-Term Memory (LSTM) neural network to predict stock trends.
The application is built using Streamlit for the frontend, Prophet/TensorFlow and Keras for the model, and various other libraries for data handling and visualization.


## Features
LSTM Model
  - Load stock data from Yahoo Finance.
  - Train an LSTM model/Prophet model on historical stock data.
  - Predict future stock prices.
  - Visualize the actual vs. predicted stock prices.
  - Interactive Streamlit interface to select stocks and prediction parameters.

## Dependencies

To run this project, you need the following Python libraries:

- `streamlit`
- `yfinance`
- `pandas`
- `numpy`
- `keras`
- `tensorflow`
- `matplotlib`
- `fbprophet`
- `plotly`

You can install these dependencies using the following command:

```bash
pip install streamlit yfinance pandas numpy keras tensorflow matplotlib plotly fbprophet
```

## Usage

1. Run the Streamlit app:
   ```bash
   streamlit run main.py
   ```
   OR
   
   ```bash
   streamlit run Predict.py
   ```bash

3. In the Streamlit interface:
   - Select a stock from the dropdown menu.
   - Choose the number of days/years for prediction using the slider.
   - View the raw data, the training results, and the predictions.

## Code Explanation

- **Data Loading:** The app loads historical stock data from Yahoo Finance using the `yfinance` library.
- **Data Preprocessing:** The data is split into training and testing sets. A TimeseriesGenerator is used to create sequences for the LSTM model.
- **Model Training:** An LSTM/Prophet model is defined and trained on the training data.
- **Prediction:** The trained model predicts future stock prices.
- **Visualization:** The results are visualized using Plotly, showing both the training results and future predictions.

## Results

The application displays two main graphs:
1. **Training Results:** Shows the actual vs. predicted stock prices on the test data.
2. **Future Predictions:** Shows the predicted stock prices for the specified number of future days.

## Project Demonstration

![Landing Page](img/01.JPG?raw=true "Landing Page")

### Prophet Model Demonstration

![Stock Interface](img/02.JPG?raw=true "Stock Interface")

![Actual Stocks](img/03.JPG?raw=true "Actual Stocks")

![Predicted Stocks](img/04.JPG?raw=true "Predicted Stocks")


### LSTM Model Demonstration

![Stock Interface](img/05.JPG?raw=true "Stock Interface")

![Actual Stocks](img/06.JPG?raw=true "Actual Stocks")

![Predicted Stocks](img/07.JPG?raw=true "Predicted Stocks")


## REFERENCES
• [https://www.geeksforgeeks.org/machine-learning/](https://www.geeksforgeeks.org/machine-learning/)
• [https://www.youtube.com/watch?v=GwIo3gDZCVQ](https://www.youtube.com/watch?v=GwIo3gDZCVQ)
• [https://finance.yahoo.com/most-active](https://finance.yahoo.com/most-active)
