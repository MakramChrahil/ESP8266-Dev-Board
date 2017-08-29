# ESP8266-Dev-Board
## Description
To get started with the ESP8266 I found a development board, which has already several components integrated. These are:  

1 Relais  
1 DHT11 temperature and humidity sensor  
2 switches  
1 potentiometer to generate different voltage at the ADC pin  
1 buzzer  
1 RGB LED  

On the board there is also a usb/serial converter to directly connect the board to the PC and a voltage regulator, which generates the 3.3V for the ESP chip. You can get it at eBay or Aliexpress starting 15$. It comes with the ESP module.  

The unit consists of 2 boards. One is the ESP8266 module without all the peripherals and usb/serial chip. This board can be purchased also separately for about 4$.  

It is breadboard friendly and has an antenna connector. The second board does have all the other components. The different components on the board can be enabled separately using some DIP switches. All external pins of the ESP module are also accessible via pins on the board. So you cannot only work with the on board components.  

The USB/serial converter on this board is a CH-341 chip. It did work out of the box on Debian Linux, but not on OSX and Windows. Drivers for thees operating systems can be downloaded here:  
OSX:       https://goo.gl/gDHtB8  
Windows :  https://goo.gl/cJ3QDm  

Unfortunately this development board comes without any documentation. I was also unable to find any on the internet. With try and error I was able to find out most of the things. The only thing I was not able to get working is the red LED. May bee there is something broken on my board. If you have something to add – please et me know.  

| FUNCTION      | NODEMCU PIN NUMBER | ESP8266 GPIO	DIP  | SWITCH NUMBER TO ENABLE |
| ------------- | -------------      | -------------     |-------------            |
| Relais        | 0	                 |  16               |   5                     |
| RGB LED green | 7                  |13                 |   2                     |
| RGB LED blue  | 6                  |12                 |   3                     |
| Buzzer        | 1                  |5                  |   5                     |

## Switches  

Switch 1 ON/OFF switch  
Switch 2 nodemcu 3  
Switch 3 nodemcu 4  

## DIP switches  

DIP SWITCH	FUNCTION  
1	RGB LED Red 
2	RGB LED Green  
3	RGB LED Blue
4	White LED
5	Relais
6	Buzzer
7	has to be always one
8	turn on to flash firmware

## On board DHT11 / DHT22

Pin2 in nodemcu firmware (GPIO 4)
