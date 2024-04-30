[Home](/index.md)

# **Component Selection**
### Final Components Summary Table
|Component| |Selection Rational
|----------|----------|----------|
|Humidity Sensor: ‎SHT40-AD1B-R3‎|![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/9bb0ee2d-dd44-47c0-adf8-2fb02f2b2c0c)| The SHT40-AD1B-R3 sensor is chosen for its outstanding performance in accuracy, wide operating range, low power consumption, and durable construction. Its precision ensures reliable data in varied conditions, while its energy efficiency extends device life. With robust build quality, it's ideal for demanding environments, making it the top pick for my application.|
|Temperature Sensor: TC74A4-3.3VCTTR|![image](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157083379/30224660-a336-4b5d-ab6f-39bdf9f647af)| - Low cost, ease of integration via the I2C interface, affordable and compact size.|
|Motor: B08PBQ1N1G|![asfd](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/692e1d20-b53f-479a-990b-2d4410b456cb)| - Compact size, sufficient power for effective vapor dispersion, quiet operation, energy efficiency, availability, and cost-effectiveness.|
|Motor Driver: IFX9201SGAUMA1|![P-PG-DSO-12](https://github.com/Team-309-Weather-Station/EGR314-Spring2024-Team309.github.io/assets/157051756/84ac50de-2263-4a08-88df-7c9a837b23b7)| - Large enough to solder by hand without damaging the component. Handles a much higher voltage and current than our product will use, lowering the risk of overloading.|
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
