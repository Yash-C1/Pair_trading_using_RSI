# Pair_trading_using_RSI

The project is about developing a pair trading model based on indicators to evaluate the strategy on the available historic data of nifty fifty.
The most important step in pairs trading is identifying the pairs with the highest correlation of
one instrument to another. In this case, the correlation is established based on the closing prices
of the nifty fifty stocks over past few days. Several indicators like moving averages, RSI, and
momentum oscillators can be used to identify ideal entry and exit conditions in the stock market.

* Total profit or loss on different pairs are calculated based on an initial investment of 1,00,000 rupees.
* Firstly for analysing the dataset easily we rearranged the given data set in vertical format and
then calculated the values of correlation ratio between all possible pairs of companies using
correlation matrix. The rearranged dataset and correlation matrix developed on the available
dataset are visualized in the below figures-  
Rearranged dataset-  
![image](https://user-images.githubusercontent.com/56033766/216749266-97b625c5-468e-4990-8391-cf92ec220188.png)  
Correlation matrix-  
![image](https://user-images.githubusercontent.com/56033766/216749304-a8d386c3-08a8-4816-8047-6a040fcfc1f9.png)  
* We used Pearson Correlation for finding correlation and stored the pairs having correlation ratio
values greater than 0.85. After that, we calculated the RSI values for each of the pairs with
correlation ratio greater than 0.85, excluding the ones that have value=1, that is the pairs which
have companies paired with themselves.  
![image](https://user-images.githubusercontent.com/56033766/216749553-3aadbf0d-3641-45a5-b8e3-26f6ced13b0c.png)  
Using these RSI values, we have calculated the
profit/loss on the closing price of those having RSI less than 30 and greater than 70. We sorted
the final pairs in descending order so that we get pairs of maximum profit.  
Sorted pairs-  
![image](https://user-images.githubusercontent.com/56033766/216749466-833a9c94-ebbc-4adb-be9b-d3152c237e9e.png)  
Calculated RSI-  
![image](https://user-images.githubusercontent.com/56033766/216749388-78d14554-b27c-484d-8abf-15e339c80760.png)  

* Plot of correlated stocks with RSI value-  
![image](https://user-images.githubusercontent.com/56033766/216749629-c37eff79-6c9b-4b1f-9433-281f1999624b.png)


* Profit/Loss was calculated for each correlated pairs taking a long position when RSI is less
than 30 and a short position when RSI is greater than 70. The exit condition is defined when
the RSI changes by 20%.
* The result show that on average 2000 INR profit can be obtained per day
over an investment of 1 Lakh INR, which accounts to nearly 2% return per day.
 
