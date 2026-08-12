# STM32H750VBT6 Development Board

## Power

It can be powered by USB-C and will be with pins in future version. It has 2 power rails due to have 2 keep noise digital from analog. i could have used ferrite beads but i have personal beef with them. 

## Digital 3.3V LDO
  AP7361C 3.3V@1A is used for Digital
  
## Analog 3.3V LDO
  TLV73333 3.3V@300mA is used for Analog parts

##   External Flash 
W25Q128- 128 MBit QSPI flash.

## MicroSD 
(473521001) is SDMMC that requires length tuning. 

## ESD Protection

TPD2EUSB30DRTR - is used for safety for DATA traces
TPD1E10B06DPYT - is used for safety of USB 5V power trace

## Buttons

#B1 and B2 is on pins PD8 and PD9 so you can add whatever function you want to those. Basically, RST button basically resets the board.


