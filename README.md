# cryptostatus
Shows a cryptocurrency informations on a i3blocks blocklet for a given time period and currency using the rate.sx API. 

Blocklet basic display:
- ![](cryptostatus.png)

## Informations
- Current price
- Currency code
- Absolute change in the selected currency 
- Percentual change 
- Period. 


## Setup / Usage

i3blocks configuration:

```
[cryptostatus]
command=$SCRIPT_DIR/cryptostatus
markup=pango
COIN=xmr                 # Cryptocurrency
CURRENCY=brl             # Reference currency
PERIOD=24h               # Period
SHOW_CHANGE=true/false   # Show change informations for the period
interval=60              # Interval between new queries
```

For the complete API reference, visit: https://github.com/chubin/rate.sx/blob/master/README.md

## Dependencies

- base gnu utilities (curl, sed, awk)
- python3


## Known Bugs/Issues and Comments

- This script is just a proof of concept and for study purposes. I know there's more efficient ways to do this (Ex: JSON)

## TODO

- Show custom icons for the coins. 
- Select more than a coin and change the display over time or by mouseclick
-  
