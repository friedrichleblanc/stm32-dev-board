# STM32H750VBT6 Development Board

## Main MCU

STM32H750VBT6 is probably an overkill for this project. But i used it anyway so i maybe use other pins if need to.
Package: LQFP-100

## Power

It can be powered by USB-C and will be with pins in future version. It has 2 power rails due to have 2 keep noise digital from analog. i could have used ferrite beads but i have personal beef with them. 

### Digital 3.3V LDO
  AP7361C 3.3V@1A is used for Digital
  
### Analog 3.3V LDO
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

## Stackup and Routing

6 layer offers improved grounding, routing space, signal integrity. Orthogonal routing strategy was partially applied.

Signal Traces/Power
\
GND Copper Pour
\
Signal Traces/Power
\
Signal Traces/Power
\
GND Copper Pour
\
Signal Traces/Power

## SWD Debugging and Programming

it has 5 pins :

BOOT0 / +3V3 / GND / PA13 / PA14

## Exposed pins

PA: PA0, PA1, PA2, PA3, PA8, PA9, PA10, PA15

PB: PB0, PB1, PB10, PB11, PB12, PB13, PB14, PB15

PC: PC0, PC1, PC4, PC5, PC6, PC7

PD: PD0, PD1, PD2, PD3, PD4, PD5, PD6, PD7, PD8, PD9, PD10, PD14, PD15

PE: PE0, PE1, PE2, PE3, PE4, PE5, PE6, PE7, PE9, PE10, PE11, PE12, PE13, PE14, PE1

also both digital and analog +3v3 and +5v. ~couple of grounds:)

## OLED interface.

SSD1306  is planned to use and have dedicated port in right side of the board.

## Clocks

ABM8G-25.000MHZ-18-D2Y-T - 25 MHZ crystal used as the main high-speed clock for the MCU

ABS07-32.768KHZ-T - 32.768 kHz crystal used for low-frequency timing and RTC.


