[Home](/index.md)

# **Component Selection**


## Humidity Sensor
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/f24cfb36-72c6-4fa4-8e4c-9128501e0bad)
| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| HIH6030-021-001 | * Low required voltage range (2.3V ~ 5.5V) <br> * I2C compatible <br> * Operating temperature -40°C ~ 100°C  | Expensive ($ 13.43) |
* Rationale: 
The HIH6030-021-001 humidity sensor was chosen for its high accuracy, wide operating range, compact design, and robust construction. It offers reliable performance across various humidity levels, is durable in harsh environments, and is supported by comprehensive technical documentation and reputable manufacturer support. These factors make it the optimal choice for the intended application.

## Temperature Sensor
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/30224660-a336-4b5d-ab6f-39bdf9f647af)
| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| TC74A4-3.3VCTTR | * Price advantage ($1.15) <br> * I2C operation <br> * Compact size  | * Limited sensing range |
* Rationale: When considering the TC74A4-3.3VCTTR temperature sensor, its low cost, ease of integration via the I2C interface, and compact size make it particularly suitable for educational purposes. Its availability from various suppliers ensures easy access for classroom projects. However, it's essential to note its limitations, such as a narrower temperature range and lower accuracy compared to some alternatives. Overall, for the situation emphasizing simplicity, affordability, and accessibility, the TC74A4-3.3VCTTR is a practical choice for achieving temperature sensor applications and basic electronics principles.
## Motor
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/b735978e-1274-4216-ba37-75f864b788ba)
| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| COM3700 | * Optimized used (water pump) <br> * Price advantage ($ 3.00)  | * Different voltage requirement (4.5V) |
* Rationale: 
The COM3700 motor pump was chosen for the humidifier due to its compact size, sufficient power for effective vapor dispersion, quiet operation, energy efficiency, availability, and cost-effectiveness, meeting project requirements efficiently.
## Motor Driver 
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/8721895b-37a0-4332-a6dc-48f48c1fe7a1)
| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| 5070 | * Multiple motors operation <br> * Less expensive per motor ($ 3.00)  | * Outputs slightly lower current <br> * More expensive unit price ($ 20.95) <br> * Larger size |
* Rationale: We decided to use the MOTORON M3S550 motor controller because it can run more than one motor. We do not yet know if we will need multiple motors, so we want to keep the option available. If we were to use the single motor controllers, we would need to purchase many more, which would use more of our budget. Although we could do this, we decided it would be better to conserve the budget as much as possible, to have more left over for unforeseen expenses.

## Voltage Regulator
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/5796ab92-032a-41f8-90e5-50b22ac70bee)
| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| LM2575-3.3WU-TR | * Simple usage <br> * 3.3V output accuracy <br> * Different Voltage output | * Secondary metarials requirement |
* Rationale: 
The LM2575-3.3WU-TR was selected for its efficiency, reliability, and ability to provide a stable 3.3-volt output, crucial for powering various electronic components. Its surface-mount TO-263 package and tape and reel packaging make it suitable for automated assembly processes, simplifying manufacturing. Overall, it meets the project requirements effectively and efficiently.
## Power Supply (Changed)
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/1a0e3f5c-9a14-4d0c-941f-7ef8ad6f0505)

| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| USE-18650-2200MAH | * High current <br> * rechargeable | * Expensive (	$4.79) |
* Rationale: 
The USE-18650-2200mAh battery was chosen for its high capacity of 2200mAh, providing sufficient power to operate the device for an extended period. Additionally, its rechargeable nature offers the advantage of long-term usability and cost-effectiveness. This combination of high current capacity and rechargeability fulfills the requirements for prolonged device operation, making it a suitable choice.

* This part is explained in power budget section.
  <br>
  <br>
  <br>

  # **Power Budget**
[Appendix D](Appendix_D.md)
