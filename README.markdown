CNCPlotter

 ![](https://github.com/lukeweston/CNCPlotter/raw/master/CNCPlotter-pcb.png)

The Freetronics CNCPlotter board is an Arduino-compatible embedded machine which incorporates two bipolar stepper motor drivers, suitable for CNC experiments and other
robotics and mechatronics applications.

The board incorporates the following hardware features:
 
- Atmel ATmega32U4 microcontroller, compatible with the Arduino Leonardo firmware, and USB connectivity to the PC. 
- 20x4 HD44780-compatible alphanumeric LCD display 
- Micro-SD card socket, for example usable for the execution of stored programs without connection to a PC. 
- Connector for a small (hobby RC aircraft style) servo motor 
- Two onboard DRV8811 bipolar stepper motor driver ICs 
- Inputs for three "limit" or "home" switches (or switches with any other kind of software-defined functionality!) 
- Connector for a cheap 4-wire resistive touchscreen, such as a Nintendo DS compatible touchscreen 
- Power supply input voltage range of 9-30V. (At least 1A current capacity is required to run the stepper motors.) 
- Output header for an optional third stepper motor driver IC, enabling three-axis CNC applications. 
 
 
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

