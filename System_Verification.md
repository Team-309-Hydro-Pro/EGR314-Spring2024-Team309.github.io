[Home](/index.md)

# **Final System Verification Matrix**

![Screenshot 2024-04-29 194341](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/3280c1c7-e5e3-4fe1-935d-b87692273170)



The motor driver, a pivotal component, is connected directly to the motor, ensuring precise control over its operation. This connection also facilitates interaction with other essential elements, mainly the temperature sensor and the ESP32 microcontroller. The temperature sensor, crucial for monitoring the system's thermal conditions, is directly linked to both the motor driver and the ESP32, enabling real-time temperature data acquisition. Meanwhile, the ESP32 microcontroller serves as the central brain of our system, receiving input from the temperature sensor and coordinating motor control through communication with the motor driver. Finally, the 3.3V regulator plays a vital role in ensuring a stable voltage supply to all main PCB connected components, with its output being shared among the microcontroller, motor driver, temperature sensor, and ESP32, thus contributing to the cohesive functioning of the entire system.
