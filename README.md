# -Build-a-Simplified-Trading-Bot-
Python bot for automated trading on Binance Futures Testnet. Test strategies, place orders, and track positions safely.


Objective:-

This project is a Python-based CLI trading bot that places Market and Limit orders on the Binance Futures Testnet (USDT-M).
It demonstrates clean project structure, input validation, logging, and proper error handling.



🚀 Features:-

Place MARKET and LIMIT orders
Supports BUY and SELL
Uses Binance Futures Testnet (USDT-M)
Command-line interface (CLI) using argparse
Input validation before sending orders
Structured logging to file and console
Clear separation of concerns (client, orders, validators, CLI)


🧱 Project Structure

trading_bot/
│
├── bot/
│   ├── __init__.py
│   ├── client.py          # Binance Futures client wrapper
│   ├── orders.py          # Order placement logic
│   ├── validators.py      # Input validation
│   └── logging_config.py  # Logging setup
│
├── logs/
│   └── trading_bot.log    # Application logs
│
├── cli.py                 # CLI entry point
├── .env                   # API credentials (not committed)
├── requirements.txt
└── README.md


Market Order:- python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.004

Market Order:- python cli.py --symbol BTCUSDT --side BUY --type LIMIT --quantity 0.004 --price 30000

📊 Output Example:- 

===== ORDER RESULT =====
Order ID     : 123456789
Status       : NEW
Executed Qty : 0
Avg Price    : N/A
========================

🛠️ Technologies Used:-

Python 3.x
python-binance
argparse
logging
dotenv
