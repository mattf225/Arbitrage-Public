# This is an internal Sports Trading tool for Caesars Sportsbook.

## What is arbitrage betting?
Arbitrage betting (otherwise known as ‘arb betting’) is an increasingly popular sports betting strategy where the bettor covers all possible outcomes. Regardless of the outcome of a match, you can guarantee a profit.

If you get it right, it essentially means that your bet cannot lose. 

## How does the tool work?
This tool uses a couple different API's to pull in Live betting data from Caesars Sportsbook, as well as approximately 50 other sportsbooks.

It then compares our odds (Caesars) for every different bet that we offer and compares it against the equivalent market of the other sportsbooks.

If our odds compared against the odds of our competitor offer an arbitrage opportunity, that bet and the details around it will be shown in the table.

The table automatically updated every minute.

## How is the code structured?

### Server Side
I use Axios on the server side to pull in the data from the appropriate API's.

Socket.io will then emit that data to the client side of all open sockets. This is sent on a 1 minute interval.

### Client Side
The client side JavaScript will then update the table with the new data.



Below are a couple screenshots of the application. Thank you for your time!



![with_arbs3](https://user-images.githubusercontent.com/93163082/169880288-3cb09e61-2a11-4940-8607-8a3625321c0f.png)


![with_arbs](https://user-images.githubusercontent.com/93163082/169875822-77eef13f-27ed-45f2-af33-0599492534ea.png)


![checking](https://user-images.githubusercontent.com/93163082/169905553-b0518a34-114a-4ee4-8841-b170cebd7338.gif)





