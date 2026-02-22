# Trady
A simple extension / application to help traders quickly make trades. It will enable traders to reduce impact cost and increase profitability. This application will be primarily focused on discritionary options traders. 
We will be focused on Nifty, Bank Nifty and Sensex optiions, because they have the highest number of participants and potential for growth.

## Normay order placement journey
* Select the strike price
* Enter the quantity
* Enter the price
* Select the order type
* Place the order

### The disadvantages of this approach:
Option prices are extremely volatile. Eg For 'ATM call or put options', In less than 1 or 2 seconds, the prices can move 3-5 rupees or sometimes even upto  10 rupees.
A normal 'Limit' order placement will take 4-5 seconds - if you don't make any typing mistake and if there is no lag in the broker terminal or app and the charts are functioning properly.
If a trader is placing an order of 500 qty and from the time the decision has been taken and the order has been placed, the price changed by 5 rupees. The impact cost will be 5*500 = Rs2500.
As the number of trades increases, the impact cost also increases significantly.
Also if a trader is placing market order, because of volatility and fluctuations, we can never be certain aboout the price at which the order will get excecuted.


## Our Approach:
The brokers provide a login feature and we can make use of this feature to provide a login option to connect to their brokerage accoount.
We will provide a settings menu where all the choice of 'strike price' , 'quantity', 'order type' and 'price increment' can be selected before the markets open at a convenient time.
We will provide a button that will be hovering over the broker's platform. The trader will click on the buy or sell button based on is his requirements. 
If the trader has selected the 'Limit order',when the trader clicks on the buy or sell button. Our algorithm bust fetch the current price of the option and place the order.
at the current price or if the trader has selected an increment number , then add that to the current price and place the order. Eg:- Current price = 300, increment is 1 then a limit order trade will be placed at Rs 301.
We will also provide a 'time feature' where if the the order is not excecuted by 30 or 60 seconds, it gets cancelled or it will fetch the current price again and place a new order.This will be helpfull in exiting the trade.
