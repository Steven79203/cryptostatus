# cryptostatus
Shows a cryptocurrency informations on a i3blocks blocklet for a given time period and currency using the rate.sx API. 

Blocklet basic display:
- ![](cryptostatus.png)

- COIN          = Cryptocurrency code
- PRICE         = Final price for the period
- CURRENCY      = Currency code
- CHANGE_ABS    = Absolute change in the selected currency 
- CHANCE_PERC   = Percentual change 
- PERIOD        = Time range. 


## Setup / Usage

i3blocks configuration:

```
[cryptostatus]
command=$SCRIPT_DIR/cryptostatus
COIN=xmr
CURRENCY=brl
PERIOD=24h
interval=60
markup=pango
```

For the complete API reference, visit: https://github.com/chubin/rate.sx/blob/master/README.md

## Dependencies

- base gnu utilities (curl, sed, awk)
- python3


## Known Bugs/Issues and Comments

- This script is just a proof of concept and for study purposes. I know there's more efficient ways to do this (Ex: JSON)
- The regex filtering is a workaround to show the proper text color since the i3blocks only parses pango markup. ANSI color codes are show as unparsed literal strings.
- Some combinations of currencies/cryptos may break the regex patterns that filter the ANSI codes from the terminal.


## TODO

- Select more than a coin to alternate the displays over time

