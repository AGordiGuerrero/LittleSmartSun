# Little Smart Sun

Arduino light dimmer for AC filament lamps. 

Developed to produce a smooth sunrise and sunset for a small [canary birds](https://en.wikipedia.org/wiki/Domestic_canary) farm, using the natural sunlight when possible.
<p align="center">
<img width="600" src="https://user-images.githubusercontent.com/10839138/115840518-10090c00-a41c-11eb-8730-bbcfc3d85c72.jpeg">
</p>

Controlled with Real Time Clock (RTC) to keep date and Light Dependent Resistor (LDR) to turn off light, if ambient light is enough.

Developed in 2014 for a farm without internet connection. Nowadays it could be easily improved using ESP32 or ESP8266.

## Features
	
- Control the amount of light of a 220VAC lamp.

- Select the time of two dimmings in 24h cycles, choosing "sunrise" and "sunset" times.

- Turn off the light in case of enough ambiental light, with a regulated threshold.

## Included
  
  - Turn off light off when a given threshold is readed via an analog input pin.
  
  - Switch for on/off the light sensor (LDR) functionality.
  
  - Switch for on/off the timer functionality.
  
  - Read the sunrise and sunset time from potentiometers.
  
  - Implement the dim control using the actual hour and using the lectures for sunrise and sunset times.
  

## Development details

- Arduino ProMini 5V board.

- RTC I2C module with battery to keep date without power.

- 5V power supply using a recycled mobile phone charger.

- Simple circuitry without devoted PCB. Just point to point soldering and wires.

- Cheap LDR to measure the amount of ambient light.

- Both the timer and the light threshold detector can be disabled with ON/OFF switches.

- Internal button for setting the clock time to 12:00h after pressing 3 seconds. 
  
- 100 dim levels (freqStep=100) but only using levels from 20 till 80 (to ensure a real effect on the light of an incandescent bulb)

- Light threshold, sunrise, and sunset times are selected with simple potentiometers.
<p align="center">
<img width="600" src="https://user-images.githubusercontent.com/10839138/115838512-0da5b280-a41a-11eb-8cb8-5392a2b8cd71.png">
</p>

## User Controls

- General ON/OFF switch.

- Light Sensor ON/OFF switch.

- Off Level threshold potentiometer.

- Timer ON/OFF switch.

- Sunrise time potentiometer.

- Sunset time potentiometer.

Conections are described in the Arduino code.

A view of the label:
<p align="center">
<img width="600" src="https://user-images.githubusercontent.com/10839138/115839487-fdda9e00-a41a-11eb-9f05-97c9e8c37c66.png">
</p>


## Based on

[Instructables Arduino Controlled Light Dimmer](https://www.instructables.com/Arduino-controlled-light-dimmer-The-circuit/)

More details at: [Litte Smart Sun at Smart Open Lab](https://www.smartopenlab.com/proyecto/little-smart-sun/)


