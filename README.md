# Greenhouse
> Working with micro-controllers, sensors and actuator

![GreenHouse](greenhouse.jpg?raw=true)

# Overview
In the IoT system, It is essential to understand the environment and make changes to the environment. In this chapter, we will learn how to work with sensors and actuators.

# Project 1
A greenhouse manager requests us to design a system that maintains the greenhouse temperature and humidity within the specified range. Besides, The system must automatically fill in water into the greenhouse whenever it is needed. This system should display the ambient temperature and humidity on the screen and turn on the air conditioner when needed.

![Schema](schema.png?raw=true)
## Requirements
Above figure shows a deeper look at the described project, we can understand the project is composed of:

 1. One sensor to get environment's temperature. i.e., BMP 280 sensor.
	 - BMP 280 is a sensor that can get the temperature, humidity and pressure of the environment with a good precision
 2. One sensor to get the environment's humidity. i.e., again BMP 280 sensor.
 3. One LCD to display necessary information. i.e., a 1-inch OLED display for the prototype (SSD1306).
 4. One Air conditioner. i.e., a DC motor for the prototype.
 5. One actuator to turn on or off the Air conditioner.
 6. One push button to disable or enable the system.
 7. One Buzzer
 8. One LED to show the running status.
 9. One Micro Controller. i.e., Arduino or Raspberry Pi. 
 10. Wires, Resistances, Breadboard (for the prototype), etc. 

# LAB 1
In this lab we learn:
 - [x] Micro-Contoller
 - [x] Digital Signal and how to Read/Write in a Micro Controller
 - [x] Analog Signal and how to Read/Write in a Micro Controller
 - [x] PWM 
 - [x] LED
 - [x] Arduino
 - [x] Arduino IDE
 - [ ] Extra: Relay
 - [ ] Extra: Fritzing

## Step 1: Turning on/off an LED
In this step, we work on the simplest part of the project. 
A LED has two pins. Cathode (+) and Anode (-). To turn on a LED, we need to put it into an Electronic circuit.
![LED](LED+bb.png?raw=true)
### Breadboard
> A breadboard is a construction base for prototyping of electronics. Because the solderless breadboard does not require soldering, it is reusable. This makes it easy to use for creating temporary prototypes and experimenting with circuit design.
> 
In The above figure, you can see a breadboard design:

 - [A, D]: bus strips. Each row is connected horizontally—usually the blue one for ground and the red one for a supply voltage.
 - [B, C]: Terminal strips. All five pins in each column are connected together. 

## Step 2: Turning on/off an LED
In this step, we connect LED to the Micro-Controller.
 ![Schema-LED](schema-LED.png?raw=true)
 Before continuing, we need to know more about the element used in this section.
### Micro-Controller
> A microcontroller is a small computer on a single integrated circuit (IC) chip. A microcontroller contains one or more CPUs (processor cores) along with memory and programmable input/output peripherals.
 
In this lab, We use an Arduino UNO development board. 
#### Device Summary
-   Operating Voltage: 5 Volts
-   Input Voltage: 7 to 20 Volts
-   Digital I/O Pins: 14 (6 provide PWM output)
-   Analog Input Pins: 6
-   DC Current per I/O Pin: 20 mA
-   DC Current for 3.3V Pin: 50 mA
-   Clock Speed: 16 MHz
-   Micro controller: ATmega328P
-   USB connection

#### Pin definition

![Arduino Pin](Arduino-Uno-Pin-Diagram.png?raw=true) 

Now, It is necessary to model the work.

![Schema-LED](LED_micro.png?raw=true)

Before continuing:
|Ex.1| Test your LED by connecting the orange wire to the red bus (VCC). Is it work? Document it in your GitHub repository using [this format](https://github.com/efrei-paris-sud/2019-sample-project/tree/master/lab/1). |
|--|--|

## Step 3: Program a Micro-Controller
In this LAB, we will use Arduino IDE. However you can use any software as you want.   [Download Arduino IDE](https://www.arduino.cc/en/Main/Software)
[How to install Arduino](Install%20Arduino.pdf?raw=true)
[Simple Program: LED Blink.ino](led_blink.ino)
If you need help on arduino language. [Arduino Language Reference](http://wiring.org.co/reference/)
