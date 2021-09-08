# Harold's A Whale
![image](https://user-images.githubusercontent.com/80294571/130271169-f94864cc-1a4b-47f3-b1c1-28081d8b4c48.png)

### Table of Contents:
[Background](https://github.com/jharvey09/Harolds_A_Whale#background)

[Steps](https://github.com/jharvey09/Harolds_A_Whale#steps)

[Historical Data](https://github.com/jharvey09/Harolds_A_Whale#resources)


### Index:
[Quatitive Analysis](https://github.com/jharvey09/Harolds_A_Whale#conduct-quantitative-analysis)

[Performance Analysis](https://github.com/jharvey09/Harolds_A_Whale#performance-analysis)

[Risk Analysis](https://github.com/jharvey09/Harolds_A_Whale#risk-analysis)

[Box Plot](https://github.com/jharvey09/Harolds_A_Whale#box-plot)

[Standard Deviation](https://github.com/jharvey09/Harolds_A_Whale#box-plot)

[Risky Portfolio](https://github.com/jharvey09/Harolds_A_Whale#which-portfolios-are-risker)

[Annualized Standard Deviation](https://github.com/jharvey09/Harolds_A_Whale#annulaized-standard-deviation)

[Rolling_Statistic](https://github.com/jharvey09/Harolds_A_Whale#rolling-statistics)

[Calculate/Plot Correlation](https://github.com/jharvey09/Harolds_A_Whale#calculateplot-correlation)

[Rolling Statistic Exponetially Weighted Average](https://github.com/jharvey09/Harolds_A_Whale#calculateplot-correlation)

### Background:
I will be creating a Retirement Planning tool; that will use the Alpaca API to grab historical closing prices for a projected retirement portfolio.  The portfolio will be composed of stocks and bonds, later running a few different Monte Carlo simulations to predict the portfolio performance at 30 years. 

### Steps:
First, read and clean several CSV files for analysis using Pandas as a DataFrame. Be ready to convert the dates to a DateTimeIndex. Next, detect and remove null values. If any columns have dollar signs or characters other than numeric values, remove those characters and convert the data types as needed. Join the CSV into a single DataFrame with columns for each portfolio's returns.

![image](https://user-images.githubusercontent.com/80294571/130269292-d984f1de-1727-44f1-8d5c-992c5766cbc1.png)

#### Conduct Quantitative Analysis:
Analyze the data to see if any portfolios outperform the stock market (i.e., the S&P 500).
#### Performance Analysis:
Calculate and plot the daily returns of all portfolios.
Calculate and plot cumulative returns for all portfolios. Does any portfolio outperform the S&P 500?

![image](https://user-images.githubusercontent.com/80294571/131744280-bf6d6209-311f-4070-9afe-b8004406e253.png)

![image](https://user-images.githubusercontent.com/80294571/131744429-513216b4-8d35-442e-b268-fb0decff9d53.png)

#### Risk Analysis:
Create a box plot for each of the returns.
Calculate the standard deviation for each portfolio.
Determine which portfolios are riskier than the S&P 500.
Calculate the Annualized Standard Deviation.

##### Box Plot:
![image](https://user-images.githubusercontent.com/80294571/130270185-033310ed-9278-404b-b065-1ad08b5afe35.png)

##### Standard Deviation:

![image](https://user-images.githubusercontent.com/80294571/131744693-e02eb9e1-4173-4940-9052-5d7e1b5c2823.png)

##### Which Portfolios Are Risker?:

![image](https://user-images.githubusercontent.com/80294571/131744924-004b2806-b385-4352-ac98-f09eaa83d9b4.png)

##### Annulaized Standard Deviation:

![image](https://user-images.githubusercontent.com/80294571/131745156-603e4c5f-a20f-4bf3-8eec-37757702c8e8.png)


#### Rolling Statistics:
Calculate and plot the rolling standard deviation for all portfolios using a 21-day window.
Calculate and plot the correlation between each stock to determine which portfolios may mimic the S&P 500.
Choose one portfolio, then calculate and plot the 60-day rolling beta between it and the S&P 500.

##### 21 Day Rolling Standard Deviation:
![image](https://user-images.githubusercontent.com/80294571/131745317-38fadd81-a392-4ac7-9ab2-af15c58c353b.png)

##### Calculate/Plot Correlation:

![image](https://user-images.githubusercontent.com/80294571/131745702-4a284bb4-3d2b-4109-9b06-ce34bfa7a3f1.png)

#### Rolling Statistics Challenge: Exponentially Weighted Average
An alternative method to calculate a rolling window is to take the exponentially weighted moving average. Also, like a moving window average, but it assigns greater importance to more recent observations. 

![image](https://user-images.githubusercontent.com/80294571/131745994-0958ca03-3c29-4b3e-a839-439bac5fdd95.png)

#### Sharpe Ratios:
Investment managers and their institutional investors look at the return-to-risk ratio, not just the returns. 
If; you have two portfolios that each offer a 10% return on investment. Yet one is lower risk; which portfolio would be the best fit?

![image](https://user-images.githubusercontent.com/80294571/131746109-81fd3c52-1293-4da3-9d10-f44efe1eb7e8.png)

#### Historical Data:
[APPLE CSV](https://github.com/jharvey09/Harolds_A_Whale/blob/main/aapl_historical.csv)

[ALGORITHMIC RETURNS](https://github.com/jharvey09/Harolds_A_Whale/blob/main/algo_returns.csv)

[COSTCO](https://github.com/jharvey09/Harolds_A_Whale/blob/main/cost_historical.csv)

[GOOGLE](https://github.com/jharvey09/Harolds_A_Whale/blob/main/goog_historical.csv)

[S&P500](https://github.com/jharvey09/Harolds_A_Whale/blob/main/sp500_history.csv)



