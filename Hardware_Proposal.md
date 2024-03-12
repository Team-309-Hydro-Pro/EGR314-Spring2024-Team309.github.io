[Home](/index.md)


# **Hardware Proposal**

![asdf](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/d5491f57-bf2c-41ee-8ec9-2ceee4ae5f34)


Voltage regulation consists of two main rails, a 4.5 V and a 3.3 V rail. The higher voltage satisfies the voltage requirement for the motor power while the 3.3V rail powers the rest of the product components. The voltage regulator also consists of a fuse. The inclusion of a fuse and the separation of voltage regulators should allow for a safer design for users to avoid using drop voltage methods that may heat up more than anticipated. This also adds an additional separation that may avoid a power surge between those two rails.
The temperature sensor and humidity systems are applied with recommendations from the developers themselves. Following their I2C set up helps create a closer resemblance to the intended company design for safer applications while the I2C limits our main data uses are limited to the two input data rails I2Cs use.
The motor driver consists of a motor pump that has a motor powered by 4.5V and a driver powered by 3.3V. Since our motor pump only intends to push outward, we applied LEDs that will activate when the motor intends to activate backward without actually doing so as a representation that can satisfy the project bidirectional motor needs.
The ESP32 system has a design that allows for simple connection set up that will ultimately allow users to edit the parameters via wi-fi. Along with an LED, the system allows for debugging that helps maintain reliable connection and function for continuous use.



## Bill of Materials

Details to [Appendix D](/Appendix_D.md)
