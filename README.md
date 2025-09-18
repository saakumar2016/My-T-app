# Dhan Desktop Trading App

This is a desktop trading application that uses the Dhan API. It is built with Node.js, Express, React, and Electron.

##
<!-- AUTO-GENERATED-CONTENT:START (625-README_ENTRY) -->
<br>

<h1 align="center">
    <img src="https://github.com/dhan-co/dhanhq-python/blob/main/dhanhq.png" width="150px" />
    <br>
    <b>DhanHQ API</b>
</h1>

<p align="center">
    Official Python client for DhanHQ trading APIs.
    <br>
    <a href="https://dhanhq.co/docs/py-dhanhq" target="_blank"><strong>Explore DhanHQ Python Client docs »</strong></a>
    <br>
    <a href="https://dhanhq.co/docs/" target="_blank"><strong>Explore DhanHQ API docs »</strong></a>
    <br>
    <a href="https://github.com/dhan-co/dhanhq-python/issues" target="_blank">Report a bug</a>
    ·
    <a href="https://github.com/dhan-co/dhanhq-python/issues" target="_blank">Request a feature</a>
    ·
    <a href="https://community.dhan.co/" target="_blank">Ask a question</a>
</p>

## Superfast Investing & Trading API
DhanHQ APIs are built for superfast trading and investing. You can use it to build your own trading platform, integrate with your existing services or simply automate your trades.

- **Completely Free APIs**: No charges for API usage, no hidden fees.
- **Real-time Market Data**: Access real-time market data for stocks, options & futures.
- **Blazing Fast Order Execution**: Place orders in milliseconds with our high-speed API.
- **Extensive Historical Data**: Get historical data for stocks and derivatives.
- **Secure & Reliable**: Your data is safe with us. We use the latest encryption standards.

## Getting Started

### Installation
```bash
pip install dhanhq
```

### Get your API Access Token
You can get your API access token by visiting [DhanHQ API docs](https://dhanhq.co/docs/pages/get-access-token/).

### A simple example
```python
from dhanhq import dhanhq

# a client_id and access_token are required to get started
dhan = dhanhq("client_id", "access_token")

# Get the list of all exchanges
dhan.get_exchange_list()

# Get the list of all segments for an exchange
dhan.get_exchange_segment_list("NSE")

# Get the list of all securities for a segment
dhan.get_securities_list("NSE", "EQUITY")

# Place an order
dhan.place_order(
    security_id="1333",
    exchange_segment="NSE_EQ",
    transaction_type="BUY",
    quantity=1,
    order_type="MARKET",
    product_type="INTRADAY",
    price=0,
)
```

## API Documentation
You can find the complete API documentation at [DhanHQ API docs](https://dhanhq.co/docs/).

<br>

<!-- AUTO-GENERATED-CONTENT:END *-->

## Features
- Login & API Key setup
- Live market data dashboard
- Place Market & Limit Orders
- View Open Orders, Positions, and Trade History

## Tech Stack
- **Backend**: Node.js + Express
- **Frontend**: React.js
- **Desktop Packaging**: Electron.js
- **Other**: WebSocket, axios, dotenv

## How to run in development mode
```
npm run dev
```

## How to build
```
npm run build
```