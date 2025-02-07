# NBIStockForecast

Project for McHacks12 hackathon @ McGill University, Winter 2025. See [Devpost](https://devpost.com/software/nbistockforecast).
Attempt to predict short term behaviour (up, down, stay) of stock prices using Machine Learning.

## Machine Learning Model
An LSTM (Long short-term memory) model was used as it is widely recognized as being performant for time series forecasting problems such as stock price prediction. 

## Methodology
We trained the LSTM model using PyTorch on datasets provided by the National Bank of Canada. These datasets included columns such as stock price, volume, bid/ask prices, and timestamps with microsecond precision. 
The frontend was developed with Dash, combining interactivity with clean visualizations powered by pandas, numpy, and plotly.

## Challenges 
One of the key challenges was handling the high-frequency data provided, especially with timestamps at the microsecond level.
Preprocessing this data to remove noise and align it effectively for training required significant effort. 
Indeed, we spent most of our time on the preprocessing of the dataset. 
Additionally, optimizing the LSTM model to avoid overfitting while maintaining real-time prediction capabilities presented another layer of complexity.

## Results
Training our model showed promising results; the model predicted whether or not the price would go up, down or stay better than random selection.
There is more to be done in order to obtain further results (more training, tuning the model, etc.)



