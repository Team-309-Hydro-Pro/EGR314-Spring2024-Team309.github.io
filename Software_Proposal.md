[Home](/index.md)

# **Software Proposal**

![Software_Proposal drawio](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/25cd78c9-edee-48e0-b182-057ef2b2f4b1)

We have several subsystems with different functionalities, including temperature and humidity sensor, as well as motor subsystem. At the beginning of main function, an initialize system is required to setup all components. Then interrupts is enabled to convert the value of two sensors into actual data we need. Based on tha data, it goes into condition function. The motor subsystem will be triggered within the temp and humidity sensor value limit, or disabled when out of limit. Finally it would return and read values again. 
