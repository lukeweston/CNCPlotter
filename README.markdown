CNCPlotter

 ![](https://github.com/lukeweston/CNCPlotter/raw/master/CNCPlotter-pcb.png)

Assuming you're using an Arduino Leonardo bootloader, the following is the mapping of Arduino pins to hardware functions.	

D0: UART RXD (not used, broken out to spare header)	
D1: UART TXD (not used, broken out to spare header)	
D2: LCD Strobe (Data loaded serially from AVR into 8-bit latch. Same as Pebble LCD hardware.)	
D3: LCD Data	
D4: LCD Clock	
D5: Z-axis direction (not used in most cases)	
D6: SD Card SPI chip select (active low). Standard SPI hardware (MOSI, MISO, SCK) used for SPI communications with SD card.	
D7: Z-axis limit switch input (not used in most cases)	
D8: Y-axis step signal	
D9: Y-axis direction signal	
D10: X-axis step signal	
D11: X-axis direction signal	
D12: Servo motor PWM position signal	
D13: Z-axis step signal (not used usually)	

A0: Touchscreen 1	
A1: Touchscreen 2	
A2: Touchscreen 3	
A3: Touchscreen 4	
A4: Y-axis limit switch input	
A5: X-axis limit switch input	

