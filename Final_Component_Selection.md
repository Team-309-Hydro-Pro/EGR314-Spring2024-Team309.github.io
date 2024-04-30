[Home](/index.md)

# **Component Selection**
### Final Components Summary Table
|Component| |Selection Rational
|----------|----------|----------|
|Humidity Sensor: ‎SHT40-AD1B-R3‎|![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/9bb0ee2d-dd44-47c0-adf8-2fb02f2b2c0c)| The SHT40-AD1B-R3 sensor is chosen for its outstanding performance in accuracy, wide operating range, low power consumption, and durable construction. Its precision ensures reliable data in varied conditions, while its energy efficiency extends device life. With robust build quality, it's ideal for demanding environments, making it the top pick for my application.|
|Temperature Sensor: TC74A4-3.3VCTTR|![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/30224660-a336-4b5d-ab6f-39bdf9f647af)| The TC74A4-3.3VCTTR sensor is a cost-effective solution offering seamless integration through its I2C interface, making it an affordable and compact choice. Its low cost doesn't compromise on quality, providing reliable temperature sensing capabilities. The ease of integration via I2C simplifies setup and reduces development time, while its compact size allows for flexible placement in space-constrained applications. With its combination of affordability, convenience, and compact design, the TC74A4-3.3VCTTR sensor is the optimal solution for my temperature monitoring needs.|
|Motor: B08PBQ1N1G|![asfd](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/692e1d20-b53f-479a-990b-2d4410b456cb)| The B08PBQ1N1G motor boasts a compact size and generates only minimal noise, ensuring effective vapor dispersion without causing disturbance. Its energy efficiency and cost-effectiveness further enhance its appeal, making it a practical choice for various applications. With its combination of compactness, low noise, power, efficiency, availability, and cost-effectiveness, the B08PBQ1N1G motor is the perfect solution for vapor dispersion requirements.|
|Motor Driver: IFX9201SGAUMA1|![P-PG-DSO-12](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157051756/84ac50de-2263-4a08-88df-7c9a837b23b7)| The IFX9201SGAUMA1 motor driver presents a size suitable for manual soldering without risking component damage. Its capability to manage substantially higher voltage and current levels than necessary reduces the risk of overloading, ensuring stable operation and longevity. This robustness makes it an ideal fit for our application, offering both ease of integration and enhanced safety.|
|3.3V Voltage Regulator: LM2575-3.3WU-TR|![Regulator1_image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/5796ab92-032a-41f8-90e5-50b22ac70bee)| - Efficiency, reliability, and ability to provide a stable 3.3-volt output.|
|5V Voltage Regulator: LM2576SX-5.0/NOPB|![TS5B](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/3d84b38f-868f-42b9-990a-46b6ff450d7a)| - Stable 5V output and ease of implementation required for the motor. Since this driver had to be compatible between the selected motor and the driver a capable and well ranged.|
|Power Supply: ZEUS 9V| ![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/bb07ed73-9f5c-4cf3-8236-785ff51bd75b)| - Less expensive, acceptable current requirements.|
  <br>

  Each listed component was selected with the new humidifer design in mind, hence a new order later into the semester. The main focus became creating a functioning humidifier using a humidity sensor with a responsive water pump to react accordingly and on time. Since we valued the implementation of an accurate reading for the best user experience selected mainly regulators with acceptable voltage ranges. Economic battery for the necessary current for our two voltage rails and to maintain a reasonable product pricing, while investing more into the highly accurate humidity sensor. Since the temperature was not a priority for our 1 sensor requirement design we selected a low cost and easy integration also with an I2C interface for a possible integration. Since the humidty sensor was successfully integrated, time had allowed for integration of he temperature sensor as well.
  <br>
  <br>
  <br>
Previous Version of Conponent Selection Details to [Appendix E](Appendix_E.md)

## Power Budget

Details to [Appendix D](Appendix_D.md)
