# cryptostatus-blocklet

Shows a cryptocurrency informations on a i3blocks blocklet for a given time period and currency using the rate.sx API. 

Blocklet basic display:
![](cryptostatus.png)

- COIN_SYMBOL   = Cryptocurrency code
- CURRENCY      = Currency code
- CURRENT_PRICE = End price for the period
- CHANGE_ABS    = Absolute change 
- CHANCE_PERC   = Percentual change 
- PERIOD        = Time period 


## Setup / Usage

Example i3blocks configuration:

```
[cryptostatus]
command=$SCRIPT_DIR/cryptostatus
interval=60
markup=pango
```

Edit these variables in the main script set the reference currency, crypto and time period  

Example:

```
coin = 'eth'
currency = 'usd'
period = '24h'
```

For the complete API reference, visit: https://github.com/chubin/rate.sx/blob/master/README.md

## Dependencies

- base gnu utilities (curl, sed, awk)
- python3

## Known Bugs

This script is just a proof of concept and for studies purposes.
  

