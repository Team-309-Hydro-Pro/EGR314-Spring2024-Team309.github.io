[Home](/index.md)

# **Block Diagram**

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/4210f1f2-115f-4add-82c6-c332f51b9360)



The block diagram above incorporates all required components including the MQTT Server connection, a humidity sensor as the primary sensor, a motor pump and accompanying driver for our actuating system and the PIC18 as our microcontroller. The combination of these devices ultimately allow for a responsive humidifier that can output the temperature value through the microcontroller as seen in the SDA/SCL I2C connection which ultimately displays through the MQTT wireless connection. Any required response, in our case the activation of the water pump to begin the natural waterfall for humidity, is sent from the microcontroller to the driver which controls the speed and the time the motor activates. Communication between the motor driver and the micro controller is SPI, while the connection to MQTT server is more specifically through the ESP32's capabilities of publishing and subscribing to the data.

Ultimately, most decisions such as the SPI and I2C were selected due to their compatabilites to their respective component which we selected before hand but overall we kept close to a simple structure for the best connection in a indoor-home use enviornment which demands simplicity for our users. We decided to also integrate 2 seperate power rails to accomodate for the water pump that required 5V minimum to react to the motor driver's control gate functions while still recieveing enough power to pump water through the spout.  This left 3.3V to continue to power the rest of the circuit board and it's included components. In order to implement the two required rails with the use of 9V batteries we integrated respective voltage regulators, using 2 batteries in parallel for the higher current draw in the main circuit 3.3V rail and 1 battery for the 5V rail.
