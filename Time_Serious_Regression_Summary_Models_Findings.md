# Unit 10—A Yen for the Future

### Decomposition using a Hodrick-Prescott Filter (Decompose the Settle price into trend and noise).
I have established the data for the Settle price and separated the as settle_noise and settle_trend using sm.tsa.filters.hpfilter. After that I plotted both the noise and trend shown in the graphs for the two series. 

### Forecasting Returns using an ARMA Model.
According to the the ARMA summary table the p-values of the lags are trending well above the p < 0.05 values and I would not recomend to buy this stock.

### Forecasting the Settle Price using an ARIMA Model.
Running the ARIMA summary table the p-values are greater than p < 0.05.

By plotting the 5 day forecast for the Settle Price of the Japanese Yen, the data per the line graph might not be that accurate at that the model likely needs more information to support more accurate forecasting.

### Forecasting Volatility with GARCH.
I have managed to run the 5 day forecast. 


### Based on your time series analysis, would you buy the yen now? 
No I would not. 

### Is the risk of the yen expected to increase or decrease?
It would be increasing. 

### Based on the model evaluation, would you feel confident in using these models for trading?
Yes I would feel confident using these models with more data. 

# Linear Regression Forecasting
In this notebook, I utilized Scikit-Learn linear regression model to predict Yen futures ("settle") returns with lagged Yen futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

Follow the steps outlined in the regression_analysis starter notebook I completed the following:

# Data Preparation (Creating Returns and Lagged Returns and splitting the data into training and testing data)

### Fitting a Linear Regression Model.
I created a Linear Regreission Model using model_lg. I used lg in my naming to easily identify the model I'm running. 

### Made predictions using the testing data.
I have run the prediction based on the first 20 predictions. I have also ran the code using the first 25 predictions and attempted to place the image of those results below. 
![Prediction_image](Images_2/unit-10-readme-photo.png)

### Out-of-sample performance.
I have done the Out-of-Sample using;
out_of = np.sqrt(mse)
print(f"Out of the sample RMSE: {out_of}")

### In-sample performance.
For the In-sample I constructed a DF for the Y, training data. I used in_sam to set up my DF. 

### Using the results from the linear regression:
In my analysis of the data I could not establish a clear comparison to identify if one model performed better or worse as my results ended up being the same. 

# Submission Checklist
Create Jupyter Notebooks for the analysis and host the notebooks on GitHub.

Include a Markdown that summarizes your models and findings and include this report in your GitHub repo.

Submit the link to your GitHub project to Bootcampspot.