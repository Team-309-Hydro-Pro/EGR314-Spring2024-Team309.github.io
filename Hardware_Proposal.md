[Home](/index.md)


# **Final Hardware Implementation**
## Final Schematic

![Final_Schematic](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/525ff851-ef5e-4878-be15-d7bee635eabb)


Voltage regulation consists of two main rails, a 4.5 V and a 3.3 V rail. The higher voltage satisfies the voltage requirement for the motor power while the 3.3V rail powers the rest of the product components. The voltage regulator also consists of a fuse. The inclusion of a fuse and the separation of voltage regulators should allow for a safer design for users to avoid using drop voltage methods that may heat up more than anticipated. This also adds an additional separation that may avoid a power surge between those two rails.
The temperature sensor and humidity systems are applied with recommendations from the developers themselves. Following their I2C set up helps create a closer resemblance to the intended company design for safer applications while the I2C limits our main data uses are limited to the two input data rails I2Cs use.
The motor driver consists of a motor pump that has a motor powered by 4.5V and a driver powered by 3.3V. Since our motor pump only intends to push outward, we applied LEDs that will activate when the motor intends to activate backward without actually doing so as a representation that can satisfy the project bidirectional motor needs.
The ESP32 system has a design that allows for simple connection set up that will ultimately allow users to edit the parameters via wi-fi. Along with an LED, the system allows for debugging that helps maintain reliable connection and function for continuous use.

## Final PCB Design
### Screenshots
|Front|Back|
|-----|-----|
|![PCB_Screenshot_Front](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/bc17e795-b395-4743-9c21-e543d4c01a46)|![PCB_Screenshot_Back](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/d403b212-5084-4807-89e2-62fe3b1b6392)|

### Photos

|Front|Back|
|-----|-----|
|![PCB Design_Top](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/1171be45-e810-46b9-b698-2d53fa288f01)| ![PCB Design_Bottom](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/94b15686-c06b-411a-9026-1824a7b9dc62)|

## Possible Improvements
Most improvements can be traced to the power management of the device. From the limited battery life to the large current draw relative to the amount of components used, it's apparent that a redesign may be benficial. Especially after all the knowledge and limitations of the minimum requirements to make the device work. 

## Bill of Materials

Details in [Appendix F](/Appendix_F.md)
