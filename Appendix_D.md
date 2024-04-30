[Home](/index.md)


## [Power Budget](https://docs.google.com/spreadsheets/d/1WLdgTx1jY-CqjdHZXyPzQMXlrSTJY2c_/edit#gid=1208100218)

![Screenshot 2024-04-29 194121](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/9a395968-e429-4092-9656-21a722e7f73a)


The team ended up using two batteries in parallel for the 3.3V rail and one battery for the 5V rail since mainly since the motor required different voltage draw which resulted in a seperate rail. 9V batteries were still used since they were the most accessible and they still proved to be flexible for our applications. Due to the high current draw from all the components on the PCB board, the parallel battery configuration allows for the higher current output while still keeping a voltage output the team was familiar with. The larger voltage output from the 5V rail allowed for the motor to remain within the control of the motor driver while avoiding a higher current stress by limiting to 1 battery. Ultimately, though the configuration allowed for programming and a successful demonstration of a few hours (without keeping the device on) the most significant detail would be the limited battery life the device may have with this 3 battery configuration. With such high current draws and a relatively low hourly current output our selected source has, it may be more beneficial to have inspiration from similar humidifiers that draw from an outlet or at least improve on the power source configuration.
