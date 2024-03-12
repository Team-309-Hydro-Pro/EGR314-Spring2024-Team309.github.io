[Home](/index.md)

# **Software Proposal**

![Software_Proposal drawio](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/25cd78c9-edee-48e0-b182-057ef2b2f4b1)

Initially at the main function, an initialize system is required to initialize the starting variables.  Under the initialize system, we require initializing a starter value for the temperature and humidity user settings. These will change depending on the user inputs. Then, initializing the actual humidity and temperature raw data in order to store the receiving data from sensors. Finally the motor state will also be initialized in order to account for the output of when it will be activated.

Interrupts are then enabled into the continuing loop that will mainly read any changes from user inputs to the sensor data itself. The limit values are read from the website as well as the actual values that the sensors are collecting. These two variables are then compared and the motor is triggered based on this comparison. The motor subsystem will be triggered if the sensor data of the temperature and humidity sensors are out of the temp and humidity sensor value limit placed by the user on their device and the room requires more humidity. Otherwise the motor subsystem remains disabled when still in limit. Ultimately, repeating the loop.

