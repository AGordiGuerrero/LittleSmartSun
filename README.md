# Little Smart Sun
Arduino light dimmer for AC lamps. Controlled with RTC and LDR to turn off light if ambient light is enough.

Developed to produce a smooth sunrise and sunset for a small [canary birds](https://en.wikipedia.org/wiki/Domestic_canary) farm, using the natural sunlight when possible.



**Features**
	
- Control of the amount of light of a 220VAC lamp.

- Select the time of the dimming in 24h cycles.

- Choose the "sunrise" and "sunset" times.

- Turn off the light in case of enough light in the ambient.

**Includes**

  - Adaptation to the Arduino Mini Pro board
  - Turn off light off when a given threshold is readed in a analog input pin
  - Switch for on/off the light sensor (LDR) functionality
  - Switch for on/off the timer functionality
  - Read the sunrise and sunset time from potentiometers
  - Implement the dim control using the actual hour and using the lectures for sunrise and sunset
  - Switch for set the clock time to 12:00h after pressing 3 seconds 
  - 100 dim levels (freqStep=100) but only using levels from 20 till 80 (to ensure a real effect on the light of an incandescent bulb)


**Based on**

[Instructables Arduino Controlled Light Dimmer](https://www.instructables.com/Arduino-controlled-light-dimmer-The-circuit/)


