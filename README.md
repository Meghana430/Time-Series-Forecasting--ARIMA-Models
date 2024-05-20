# Time-Series-Forecasting--ARIMA-Models

Using R programming to forecast COVID-19 Cases for the state of Connecticut, USA

The purpose of this poroject is to learn ARIMA models and then apply that knowledge to forecast Covid cases.

The time-series data on several US states on Covid cases  --- See "2020_Covid_Data.xlsx" on the course page. You can use it to train/test your models. 

Each member of your team is assigned to one US state 

Deliverable:

Daily forecast from 1st Jan 2021 through 10th Feb 2021.

 
What I have done:

Fit auto.arima (p,d,q) x (P,D,Q) model to the time series on cases for your state. You are free to consult with your friends and/or team members.
Fit alternative ARIMA models as you deem fit. You can also use Holt-Winters model if you want.
Average the forecasts from the best model and the few good ones from the subset of alternative models using aicc weights or bic weights.
The forecast horizon is 1st Jan 2021 through 10th Feb 2021. 
