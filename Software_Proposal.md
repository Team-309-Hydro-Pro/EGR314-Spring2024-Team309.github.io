[Home](/index.md)

# **Final Software UML Diagram**

![Software_Diagram](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/1e965695-f002-4723-ada9-f6fbf64a2fa5)

Initially at the main function, an initialize system is required to initialize the starting variables.  Under the initialize system, we require initializing a starter value for the humidity set value. These will change depending on the user inputs. Then, initializing the actual humidity raw data in order to store the receiving data from sensors. Finally the motor state will also be initialized in order to account for the output of when it will be activated.

Interrupts are then enabled into the continuing loop that will mainly read and write from the data transfer between the MQTT and ESP32. The integrated timer callback function (e.i. timer_callback()) increments a timer every millisecond, updating seconds when it reaches 1000 milliseconds. This timer alongside the humidty temperature are then printed wirelessly onto the MQTT server via the esp32. The limit values are read from the set value as well as the actual values that the sensors are collecting. These two variables are then compared and the motor is triggered based on this comparison. The motor subsystem will be triggered if the sensor data of the temperature and humidity sensors are out of the humidity sensor set value limits. Otherwise the motor subsystem remains disabled when still in limit. Ultimately, repeating the loop. 

### Top 5 Changes
1. Humidity sensor extra

2. using time interrupt to toggle the LED

3. user value

4.

5.

### MPLAB MCC Configuration and MQTT Topic Table in [Appendix G](/Appendix_G.md)

