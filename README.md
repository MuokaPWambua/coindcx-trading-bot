# coindcx-trading-bot
It's a nodejs trading bot that uses infinite grid trading strategy 

If you want to see backtested results checkout: 
https://github.com/adarsh-chouhan-au8/Effective-DCA-Strategy-Crypto

## How to use
### install packages
Run npm install it will install all required node modules
```
sudo apt-get install build-essential
```

### configuration
Create a mysql database and install trading_bot.sql

In pairs table each row represents a Cryptocurrency data object formed in JSON string.

Sample data object

```
{
    'name': 'chainlink',
    'pair': 'B-LINK_USDT',
    'symbol': 'LINKUSDT',
    "target_currency_precision": 2,
    'tradingUnit': 15,
    'levels': [[17.98, 'empty'], [17.61, 'empty'], [17.30, 'empty'], [16.93, 'empty']]
}
```
Here object.levels contains grid data in a 2d array.

Add as many levels and crypto pairs you require.