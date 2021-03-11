# crptstatus-blocklet

Shows cryptocurrencies informations on the i3blocks for a given time period and currency. 

Blocklet basic display:
![](example.png)

Where:
- COIN_SYMBOL   = Cryptocurrency code
- CURRENCY      = Currency code
- CURRENT_PRICE = End price for the period
- CHANGE_ABS    = Absolute change 
- CHANCE_PERC   = Percentual change 


## Setup / Usage

Example i3blocks configuration:

```
[cryptostatus]
command=$SCRIPT_DIR/cryptostatus
interval=60
markup=pango
```

Edit the main script to change which currency, crypto and time period  

```
...

coin = 'eth'
currency = 'brl'
period = '24h'

...
```

## Dependencies

- python3
