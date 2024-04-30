[Home](/index.md)


# **Final Hardware Implementation**
## Final Schematic

![Final_Schematic](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/525ff851-ef5e-4878-be15-d7bee635eabb)


The schematic's functionality is meticulously crafted to fulfill the intricate needs of users and stringent product requirements. Voltage regulation is a cornerstone, featuring two principal rails: a 3.3V rail that powers the majority of the product's components and a 5V rail specifically allocated for motor power. A pivotal decision arose at the eleventh hour, prompting the direct connection of the 5V regulator to the motor to swiftly align with project requisites. This decision, coupled with the integration of a fuse within the voltage regulator, fortifies safety measures, shielding against potential hazards stemming from drop voltage methods and power surges between the dual rails.

In tandem with safety considerations, the implementation of temperature and humidity systems meticulously adheres to developers' recommendations, ensuring not only adherence to safety standards but also steadfast reliability. Furthermore, the incorporation of a secondary temperature and humidity sensor, meticulously calibrated for precise control over air humidity, underscores the design's commitment to meeting user needs. This additional sensor proves particularly invaluable in scenarios such as humidifier applications, where meticulous humidity control is paramount for user comfort and well-being.

The motor driver section of the schematic intricately balances functionality and safety, with the strategic integration of LEDs serving as intuitive indicators of motor activation, all while circumventing the need for actual direction reversal. This nuanced approach not only meets bidirectional motor requirements but also bolsters safety by minimizing potential confusion or accidents.

Rounding out the schematic's design, the ESP32 system stands as a testament to user-centricity and ease of use. Designed for straightforward connection setup, it empowers users to effortlessly adjust parameters via Wi-Fi, fostering unparalleled convenience and control. Moreover, the integration of LEDs within the system offers invaluable debugging capabilities, ensuring seamless and uninterrupted operation under diverse circumstances.

Throughout the design and decision-making process, our team's unwavering commitment to safety, reliability, and user satisfaction has been paramount. Each element of the schematic is meticulously crafted to not only meet technical specifications but also to exceed user expectations, culminating in a product that is not just functional but truly exceptional.

## Final PCB Design
### Screenshots

|Front|Back|
|-----|-----|
|![PCB_Screenshot_Front](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/bc17e795-b395-4743-9c21-e543d4c01a46)| ![PCB_Screenshot_Back](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/d403b212-5084-4807-89e2-62fe3b1b6392)|

### Photos

|Front|Back|
|-----|-----|
|![PCB Design_Top](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/1171be45-e810-46b9-b698-2d53fa288f01)| ![PCB Design_Bottom](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/84349229/94b15686-c06b-411a-9026-1824a7b9dc62)|

## Possible Improvements
Most improvements can be traced to the power management of the device. From the limited battery life to the large current draw relative to the amount of components used, it's apparent that a redesign may be benficial. Especially after all the knowledge and limitations of the minimum requirements to make the device work. 

With the applied power rails in our circuit we also experienced several component shortages which had the team consider methods to help safely regulate these issues that can damage the board. Attention to the size of some components such as the humidity sensor would also be important to improve upon to help with the soldering and ultimately efficiency in construction of the board. Though this aspect would be more applicable if the product is hand-soldered since at a manufacturing level the size of most of our components are acceptable. There was also concern regarding the heat dissipation in from the voltage regulator as some tests did result in very hot ground plates on the regulators. Though the issue wasn't dangerous after testing our final regulator we would also look into platings or methods to help with this heat dissipation to ensure the safety of our product function and any customers.

Most of these solutions are in relation to the goal of completing the board with the constraints of the ASU 2024 showcase. For further improvements to the design as a product it would be optimal to improve the board by pushing the limits of it's size. Taking into account manufacturing methods, it would be important to push for an even smaller board for a more manageable encasing and a less expensive board. The use of an actual headers for battery ease of replacement would also be a great improvement for the customer use. 

## Bill of Materials

Details in [Appendix F](/Appendix_F.md)
