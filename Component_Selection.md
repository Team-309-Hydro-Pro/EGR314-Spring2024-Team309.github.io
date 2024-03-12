[Home](/index.md)

# **Component Selection**


## Humidity Sensor: HIH6030-021-001
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/f24cfb36-72c6-4fa4-8e4c-9128501e0bad)

| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| HIH6030-021-001 | - Low required voltage range (2.3V ~ 5.5V) <br> - I2C compatible <br> - Operating temperature -40°C ~ 100°C  | - Expensive ($ 13.43) |

* Rationale: 
The HIH6030-021-001 humidity sensor was chosen for its high accuracy, wide operating range, compact design, and robust construction. It offers reliable performance across various humidity levels, is durable in harsh environments, and is supported by comprehensive technical documentation and reputable manufacturer support. These factors make it the optimal choice for the intended application.


  <br>
  <br>
  <br>

## Temperature Sensor: TC74A4-3.3VCTTR
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/30224660-a336-4b5d-ab6f-39bdf9f647af)

| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| TC74A4-3.3VCTTR | - Price advantage ($1.15) <br> - I2C operation <br> - Compact size  | - Limited sensing range |

* Rationale: When considering the TC74A4-3.3VCTTR temperature sensor, its low cost, ease of integration via the I2C interface, and compact size make it particularly suitable for educational purposes. Its availability from various suppliers ensures easy access for classroom projects. However, it's essential to note its limitations, such as a narrower temperature range and lower accuracy compared to some alternatives. Overall, for the situation emphasizing simplicity, affordability, and accessibility, the TC74A4-3.3VCTTR is a practical choice for achieving temperature sensor applications and basic electronics principles.

  <br>
  <br>
  <br>
## Motor: COM3700
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/b735978e-1274-4216-ba37-75f864b788ba)

| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| COM3700 | - Optimized used (water pump) <br> - Price advantage ($ 3.00)  | - Different voltage requirement (4.5V) |

* Rationale: 
The COM3700 motor pump was chosen for the humidifier due to its compact size, sufficient power for effective vapor dispersion, quiet operation, energy efficiency, availability, and cost-effectiveness, meeting project requirements efficiently.


  <br>
  <br>
  <br>
## Motor Driver: IFX9201SGAUMA1
![P-PG-DSO-12](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157051756/84ac50de-2263-4a08-88df-7c9a837b23b7)

| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| 5070 | - Multiple motors operation <br> - Less expensive per motor ($ 3.00)  | - Outputs slightly lower current <br> - More expensive unit price ($ 20.95) <br> - Larger size |

* Rationale: We decided to use the IFX9201SGAUMA1 primarily because we already have several of it, so we will not need to purchase any for our prototype. It is also large enough to solder by hand without damaging the component. It also can handle a much higher voltage and current than our product will use, so there is no risk of overloading the driver.

  
  
  <br>
  <br>
  <br>
  
## Voltage Regulator: LM2575-3.3WU-TR
![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/5796ab92-032a-41f8-90e5-50b22ac70bee)

| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| LM2575-3.3WU-TR | - Simple usage <br> - 3.3V output accuracy <br> - Different Voltage output | - Secondary metarials requirement |

* Rationale: 
The LM2575-3.3WU-TR was selected for its efficiency, reliability, and ability to provide a stable 3.3-volt output, crucial for powering various electronic components. Its surface-mount TO-263 package and tape and reel packaging make it suitable for automated assembly processes, simplifying manufacturing. Overall, it meets the project requirements effectively and efficiently.

  <br>
  <br>
  <br>
## Power Supply: A1604 BK210J
![Battery](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/92e356b3-3811-432b-a5c3-394f82a8db0c)


| Subsystem Option | Strength | Weakness |
|----------|----------|----------|
| A1604 BK210J | - Sufficient current <br> - Affordable Price ($1.69) | - High Voltage (9V) |

* Rationale: 
Although option 2 is rechargeable that seems to be more convenient, the lack of capacity (250mAh) is an issue, especially when it works in the rural area with lack of charge points. Option 1 and 3 have almost exactly the same data as each other, but option 3 is less expensive.


  <br>
  <br>
  <br>

  # **Power Budget**
[Appendix D](Appendix_D.md)
