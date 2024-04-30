[Home](/index.md)

# **Final Software UML Diagram**

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/80887a45-6ffb-4259-a806-7a9e7c9f7ef8)




Initially at the main function, an initialize system is required to initialize the starting variables.  Under the initialize system, we require initializing a starter value for the humidity set value. These will change depending on the user inputs. Then, initializing the actual humidity raw data in order to store the receiving data from sensors. Finally the motor state will also be initialized in order to account for the output of when it will be activated.

Interrupts are then enabled into the continuing loop that will mainly read and write from the data transfer between the MQTT and ESP32. The integrated timer callback function (e.i. timer_callback()) increments a timer every millisecond, updating seconds when it reaches 1000 milliseconds. This timer alongside the humidty temperature are then printed wirelessly onto the MQTT server via the esp32. The limit values are read from the set value as well as the actual values that the sensors are collecting. These two variables are then compared and the motor is triggered based on this comparison. The motor subsystem will be triggered if the sensor data of the temperature and humidity sensors are out of the humidity sensor set value limits. Otherwise the motor subsystem remains disabled when still in limit. Ultimately, repeating the loop. 

### Top 5 Changes
1. Intially, for the team's main sensor we focused on implementing the temperature with the humidity sensor as an extra. Since our product was a humidifier we were really inclined to have the humidity sensor working but due to complications, we regarded the temperature sensor as the realistic application. Alongside group complications we also only required one sensor to work. Ultimately, we were able to implement the humidity sensor for a more reasonable function of the device.

2. Initially, the main application of LED were purely for debugging components but towards the ending the implementaion of the LED for the time interrupt was used to toggle the LED. This way it became more apparent when interrupt was being executed in the loop.

3. Early into the design, it was intended to have the user set the parameters at which the motor would activate on. Parameters of which would be accessed through an MQTT server for the user to change with ease. Though, the MQTT proved to be more complicated to implement for even recieving data so we began focusing on the functioning of the whole code instead of this feature.

4. Previously, we had implemented a motor delay that lasted minutes before reading data to avoid reading data constantly. This was meant to be implemented for the "disable motor" feature but was ultimately concerning to have due to the elongaded delay function that may cause issues in being stuck not reading for so long. T

5. Another change in the UML was the inclusion of a value conversion, specifically, for the temperature values. Since our design used to incorporate user input we didn't consider displaying the current temperature since we only intended to send directly to the ESP32 for the MC to read react accordingly. Though it was apparent that the converted value would be useful for the user and ultimately for debugging purposes.

## MPLAB MCC Configuration and MQTT Topic Table 
Details in [Appendix G](/Appendix_G.md)

