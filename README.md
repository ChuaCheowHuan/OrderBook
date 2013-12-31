OrderBook
=========

Matching engine based on a limit order book written in Python.

Features:
* Standard price-time priority
* Supports both market and limit orders
* Add, cancel, update orders

Requirements:
* bintrees

Key Functions
=============

process_order

cancel_order

modify_order

get_volume_at_price

get_best_bid

get_best_ask

Data Structure
==============

Orders are sent to the order book using the process_order function. The Order is created using a quote.

```python
# For a limit order
quote = {'type' : 'limit',
         'side' : 'bid', 
         'quantity' : 6, 
         'price' : 108.2, 
         'trade_id' : 001}
         
# and for a market order:
quote = {'type' : 'market',
         'side' : 'ask', 
         'quantity' : 6, 
         'trade_id' : 002}
```

