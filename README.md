# 🚀 TraderJoe BSC Sniper Bot 🚀


Web3 TraderJoe Sniper && Take Profit/StopLose bot written in python3, Please note the license conditions!
### The first Avalanche Smart Chain sniper bot with Honeypot checker!  

## If support is needed, feel free to contact me on Telegram.

[![Telegram](https://img.shields.io/badge/Telegram-@Sevens_W3_Lab-blue)](https://t.me/Sevens_W3_Lab)


# Infos
This Tool only buys/sells with/to AVAX but it use Multi Hops to get allways the best Output!  
Attention, You pay 0.77% Tax on your swap amount!  

# SUPPORT & HELP
Visit our community for help or questions, on Discord or Github you can open tickets!


# Download
### If you are not familiar with Python please have a look at [Releases](https://github.com/Sevens-W3-Lab/TraderJoe_Avax_Sniper_Bot/releases), there you can download Windows executable.

### Setup your Address and secret key in Settings.json and Run main-GUI.exe.

# Install
First of all, you need install Python3+
Run on Android you need Install [Termux](https://termux.com/) only from F-Droid works atm. 
```shell
termux: 
$ pkg install python git cmake 
Debian/Ubuntu: 
$ sudo apt install python3 git cmake gcc
Windows:
You Need to install Visual Studio BuildTools & Python3
```

### Setup your Address and secret key in Settings.json.

Clone Repo:  
```shell
git clone https://github.com/Trading-Tiger/TraderJoe_BSC_Sniper_Bot
cd TraderJoe_BSC_Sniper_Bot
```

Install Requirements:  
```python
python -m pip install -r requirements.txt
```  

Start Sniper:  
```python
python Sniper.py -t <TOKEN_ADDRESS> -a <AMOUNT> -tx <TXAMOUNT> -hp -wb <BLOCKS WAIT BEFORE BUY> -tp <TAKE PROFIT IN PERCENT> -sl <STOP LOSE IN PERCENT>
python Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 -a 0.001 -tx 2 -hp  -wb 10 -tp 50
python Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 --sellonly
python Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 -a 0.001 --buyonly
python Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 -tsl 10 -tp 10 -sl 10 -nb
```  

Here are all options with infos:  
All values of the TakeProfit, StopLoss and TrailingStoploss are in percent.
```python3
*'-t' or '--token', Token for snipe e.g. "-t 0x34faa80fec0233e045ed4737cc152a71e490e2e3"
'-a' or '--amount', float, Amount in AVAX to snipe e.g. "-a 0.1"

'-tx' or '--txamount', how mutch tx you want to send? It split your AVAX amount in e.g. "-tx 5"

'-wb' or '--awaitBlocks', default=0, Await Blocks before sending BUY Transaction. e.g. "-ab 50" 

'-hp' or '--honeypot', if you use this Flag, your token get checks if token is honypot before buy!

'-nb' or '--nobuy', No Buy, Skipp buy, if you want to use only TakeProfit/StopLoss/TrailingStopLoss
'-tp' or '--takeprofit', Percentage TakeProfit from your input AVAX amount. e.g. "-tp 50" 
'-sl' or '--stoploss', Percentage StopLoss from your input AVAX amount. e.g. "-sl 50" 
'-tsl'or '--trailingstoploss', 'Percentage Trailing-Stop-loss from your first Quote "-tsl 50"

'-so' or '--sellonly', Sell ALL your Tokens from given token address
'-bo' or '--buyonly', Buy Tokens with your given amount

* = require every time its runs!
```
## Trailing-Stop-Loss:
<img src="https://i.ytimg.com/vi/dZFb0-fwqOk/maxresdefault.jpg" height="400">
