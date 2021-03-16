# cryptostatus
Shows a cryptocurrency informations on the status bar a given time period and currency using the rate.sx API. Polybar fork

Blocklet basic display:
- ![](cryptostatus.png)

## Informations
- Current price
- Currency code
- Absolute change in the selected currency 
- Percentual change 
- Period. 


## Setup / Usage

polybar configuration example:

```
[module/cryptostatus]
type = custom/scrypt
exec = $SCRITP_DIR/cryptostatus $COIN $CURRENCY $PERIOD $SHOW_CHANGE
format = <label>
format-underline = #0000ff

```

For the complete API reference, visit: https://github.com/chubin/rate.sx/blob/master/README.md

## Dependencies

- python3


## Known Bugs/Issues and Comments

- This script is just a proof of concept and for study purposes. I know there's more efficient ways to do this (Ex: JSON)


## TODO

- Show custom icons for the coins. 
- Select more than a coin and change the display over time or by mouseclick  
