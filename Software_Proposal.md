[Home](/index.md)

# **Final Software UML Diagram**

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/80887a45-6ffb-4259-a806-7a9e7c9f7ef8)




Initially at the main function, an initialize system is required to initialize the starting variables.  Under the initialize system, we require initializing a starter value for the humidity set value. These will change depending on the user inputs. Then, initializing the actual humidity raw data in order to store the receiving data from sensors. Finally the motor state will also be initialized in order to account for the output of when it will be activated.

Interrupts are then enabled into the continuing loop that will mainly read and write from the data transfer between the MQTT and ESP32. The integrated timer callback function (e.i. timer_callback()) increments a timer every millisecond, updating seconds when it reaches 1000 milliseconds. This timer alongside the humidity temperature are then printed wirelessly onto the MQTT server via the esp32. The limit values are read from the set value as well as the actual values that the sensors are collecting. These two variables are then compared and the motor is triggered based on this comparison. The motor subsystem will be triggered if the sensor data of the temperature and humidity sensors are out of the humidity sensor set value limits. Otherwise the motor subsystem remains disabled when still in limit. Ultimately, repeating the loop. 

### Top 5 Changes
1. Intially, for the team's main sensor we focused on implementing the temperature with the humidity sensor as an extra. Since our product was a humidifier we were really inclined to have the humidity sensor working but due to complications, we regarded the temperature sensor as the realistic application. Alongside group complications we also only required one sensor to work. Ultimately, we were able to implement the humidity sensor for a more reasonable function of the device.

2. Initially, the main application of LED were purely for debugging components but towards the ending the implementaion of the LED for the time interrupt was used to toggle the LED. This way it became more apparent when interrupt was being executed in the loop.

3. Early into the design, it was intended to have the user set the parameters at which the motor would activate on. Parameters of which would be accessed through an MQTT server for the user to change with ease. Though, the MQTT proved to be more complicated to implement for even recieving data so we began focusing on the functioning of the whole code instead of this feature.

4. Previously, we had implemented a motor delay that lasted minutes before reading data to avoid reading data constantly. This was meant to be implemented for the "disable motor" feature but was ultimately concerning to have due to the elongaded delay function that may cause issues in being stuck not reading for so long. T

5. Another change in the UML was the inclusion of a value conversion, specifically, for the temperature values. Since our design used to incorporate user input we didn't consider displaying the current temperature since we only intended to send directly to the ESP32 for the MC to read react accordingly. Though it was apparent that the converted value would be useful for the user and ultimately for debugging purposes.

### Possible Improvements
The most significant change we would be interested in adding for improvement would incorporate the application of the MQTT software. Due to various connection issues in the code, we believe there was much to learn in integrating the integration of it into the software design. For example, a more user-friendly interface possibly with the implementation of a website for user access would help in various ways. One way is the application of user input that we looked forward to integrate for better humidity control. Ultimately, the MQTT proved to be difficult to apply with the time limitations and other issues to fix. 

Interrupts also proved to be troubling to implement. Though the inturrupt loop seen in the diagram seemed to be proved successful, integration of the motor control was prefered be included or at least have an interrupt for the safety of the mechanism or any undesired motor activity. With interrupts in mind, ensuring a proper handling of interrupts was also we don't believe to have spent enough time on, especially in the more time-sensitive functions. We would aim to put more time into making sure interrupt service routines are efficient and do not block for long periods as we were already having issues with longer blockings from our previous delay implementations.

Breaking the code into smaller more understandable modules and functions with clear direction is also a desired improvement. Since there was trouble sharing code withing team mates and understanding, this organization would greatly benifit the optimization of the device and maybe help with any updates as well. Some functions we can separate could be the temperature reading, humidity reading, actuator control, time tracking, and ESP32 data exchange so that they are into separate working functions. Another implementation for improved organization could the integration of set variables for constantly changed values. Instead of declaring some values for debugging within their respective function, highly accessed values could be clearly stated in the main code for increased legability.

## MPLAB MCC Configuration and MQTT Topic Table 
Details in [Appendix G](/Appendix_G.md)

