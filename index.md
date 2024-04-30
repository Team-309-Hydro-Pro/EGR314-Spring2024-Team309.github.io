Home
---
### Arizona State University | Embedded Systems Design Project II (Spring 2024) | Dr. Nichols
#### Created: 1/26/2024 (Last updated: 4/29/2024)

# Team 309 - Smart Atmospheric Humiditifier (HydroPro)

## Embedded Systems Design Project II, Group 309 (2024 Spring) 



## Team members 

* Jinuk Jeong
* Ruryck Adame Butanda
* Andrew Kleshock

## Introduction

This is the team for EGR 314 Spring 2024. In the quest for better home comfort, accuracy and simplicity are key. While professional weather stations have highly precise sensors for weather forecasting, there's a chance to bring similar accuracy and ease to everyday home devices. While mobile apps help us understand outdoor weather, there's room for improvement indoors, especially with devices like humidifiers. One such example are humidifiers which can be equipped with advanced sensors to accurately measure humidity and temperature, making indoor living more comfortable, accurate and healthy. This isn't just an idea; it's a possibility and our goal where advanced sensor technology meets user-friendly design. We offer a new way to manage home climate through HydroPro. Team 309 aims to design a weather-detecting humidifier. Hydropro is the humidifier that controls the desired humidity in the air as it constantly measures the current humidity in a room's enviornment. 

The project plans to involve the development of a weather station for these demands to a wider public. With the inclusion of a humidity sensor for a mobile weather station, the product is intended to collect and transfer data over WiFi using the MQTT protocol. The project also intends to include at least 1 actuator in the form of a water pump motor and communicate commands over a I2C or SPI-based protocol. The functionality of the motor controlled actuator will remain of high importance in this project for the most successful sensor readings. Therfore, we aim to maintain similar accuracy to competitors in the weather sensing market, including the durability they are known for having as well. 

Our main focus became individuals who specifically require the humidity control in value for their health condition. Whether it be for natural skin care necessities or more serious health conditions. We believe that higher precision in data collection can lead to the high quality humidity sensor that these people would benifit with especially for those urgent well-being practices. These individuals valuing the health benefits that come with the use of humidifiers then become our target purchasers, even if it may not be themselves specifically. Any that value indoor comfort, health, and well-being and are willing to invest in products that offer reliable performance and user-friendly features is our target demographic. With some examples being office managers, parents, Wellness Enthusiasts, etc. With such attention to value in health, we aim to offer the same attention in our customer service through mindful maintaince capabilities through design implementations of a durability, a simple user interface and a compact design. Ultimately, marketing the design is to be done by highlighting the humidifier, specifically, featuring sensors for controlling the room humidity condition for personal benefit.



## [Team organization](/Team_Organization.md)




## [User Needs, Benchmarking, and Requirements](/User_needs_Benchmarking_Requirements.md)





## [ Design Ideation](/Design_Ideation.md)


## Presentation (Checkpoint 1)


<iframe width="560" height="315" src="https://www.youtube.com/embed/tRtqgoy4ZYQ?si=hRInnPfIJlFhpfWV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>




## [Final Selected Design](/Selected_Design.md)


## [Final Block Diagram](/Block_Diagram.md)


## Final Component Selection
### Final Components Summary Table
 
|Humidity Sensor: HIH6030-021-001|![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/f24cfb36-72c6-4fa4-8e4c-9128501e0bad)| -High accuracy, wide operating range, compact design, and robust construction.|
|Temperature Sensor: TC74A4-3.3VCTTR|![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/30224660-a336-4b5d-ab6f-39bdf9f647af)| - Low cost, ease of integration via the I2C interface, affordable and compact size.|
|Motor: COM3700|![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/b735978e-1274-4216-ba37-75f864b788ba)| - Compact size, sufficient power for effective vapor dispersion, quiet operation, energy efficiency, availability, and cost-effectiveness.|
|Motor Driver: IFX9201SGAUMA1|![P-PG-DSO-12](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157051756/84ac50de-2263-4a08-88df-7c9a837b23b7)| - Large enough to solder by hand without damaging the component. Handles a much higher voltage and current than our product will use, lowering the risk of overloading.|
|3.3V Voltage Regulator: LM2575-3.3WU-TR|![Regulator1_image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/5796ab92-032a-41f8-90e5-50b22ac70bee)| - Efficiency, reliability, and ability to provide a stable 3.3-volt output.|
|5V Voltage Regulator: LM2576SX-5.0/NOPB|![TS5B](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/3d84b38f-868f-42b9-990a-46b6ff450d7a)| - Stable 5V output and ease of implementation required for the motor. Since this driver had to be compatible between the selected motor and the driver a capable and well ranged.|
|Power Supply: A1604 BK210J| ![Battery](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/92e356b3-3811-432b-a5c3-394f82a8db0c)| - Less expensive, acceptable current requirements.|

Each listed component was selected with the new humidifer design in mind, hence a new order later into the semester. The main focus became creating a functioning humidifier using a humidity sensor with a responsive water pump to react accordingly and on time. Since we valued the implementation of an accurate reading for the best user experience selected mainly regulators with acceptable voltage ranges. Economic battery for the necessary current for our two voltage rails and to maintain a reasonable product pricing, while investing more into the highly accurate humidity sensor. Since the temperature was not a priority for our 1 sensor requirement design we selected a low cost and easy integration also with an I2C interface for a possible integration. Since the humidty sensor was successfully integrated, time had allowed for integration of he temperature sensor as well.

Details to **Power Budget and Reflection** [Appendix D](Appendix_D.md)
<br>
<br>

## [Microcontroller Selection](/Microcontroller_Selection.md)


## [Final Hardware Implementation](/Hardware_Proposal.md)


## [Final Software Implementation](/Software_Proposal.md)


## [System Verification](/System_Verification.md)


## [Lessons learned](/Lessons_learned.md)


## [Recommendations for future students](/Recommendations_for_future_students.md)

## Appendix

[Appendix A](/Appendix_A.md)

[Appendix B](/Appendix_B.md)

[Appendix C](/Appendix_C.md)

[Appendix D](/Appendix_D.md)

[Appendix E](/Appendix_E.md)
