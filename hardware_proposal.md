# Hardware Implementation

## Schematic Design
The entire system was powered by 9V batteries that are connected to every other part of the system that requires power. The design utilized a switching voltage regulator that regulated voltage from 9V to 3.3V, meaning there are 2 power rails for the entire system. Most of the system was powered by the 3.3V such as the microcontroller, ADC, ESP32, hall effect sensor and OLED. However, three of the components were powered by the 9V power rail such as the voltage regulator, motor driver and motor.

## Subsystems

### Microcontroller/Voltage Regulator
  The microcontroller (PIC18F27Q10) connects to every other system on the board, including the LED array, button with pullup resistor, and ESP32. The ESP32 allows data to be sent to the MQTT server. It has 2 MSSP communication lines that can communicate with SPI or I2C components. These were used to communicate with the hall effect sensor, moisture sensor and motor driver.
  
### Hall Effect Sensor
  The Hall Effect Sensor can detect the angle of certain components and communicate with the microcontroller directly. This was used to determine the wind speed and direction. It used one of the I2C modules and was managed by Claire Rogers.
  
### Moisture Sensor
  A custom moisture sensor was made for the system which consists of two wires that hung off the board. While in water, one can be powered by the other. This information is sent to the ADC (MCP3426). This allows the team to detect whether or not the system was in water. It used one of the I2C communication lines and was managed by Jacob Pisors.
  
### Motor and Motor driver
  The motor and motor driver (IFX9201SG) both operate at 9V and function based on the information given by the hall effect sensor. It turned the sail based on the direction detected by the hall effect sensor. It used an SPI module and was managed by Abigail Gordon.
  
### Meeting User Needs
 The team met users need by using two serial sensors and a motor. The functions of those are described above and how they relate to each other. All of this information was broadcasted over WIFI for anyone to see. Since the design was a sailboat, the hall effect was used to detect wind direction then sent that information to the motor so it could adjust the sail. The moisture sensor was used to make sure that the prototype was in water which would then activate the hall effect and motor. 

## Our Schematic design

This shows the first iteration of our full Schematic:
[To Download](https://github.com/EGR314Team206/egr314team206.github.io/blob/main/SystemDesign_Sch.pdf)

## Photos of Board Design
<figure class="image">  
<p align="center">  
<img src="https://user-images.githubusercontent.com/122958638/235537237-46c90512-1312-446d-a984-f975acc3401e.png" width="40%"><br>
</p>
</figure>

<p align="center">
Figure 9.1: Top of Board Design
</p>

<figure class="image">  
<p align="center">  
<img src="https://user-images.githubusercontent.com/122958638/235537241-1025c928-b6d2-43a6-a65f-c604dcdc2c58.png" width="40%"><br>
</p>
</figure>

<p align="center">
Figure 9.2: Bottom of Board Design
</p>

## Photos of Physical Board

<figure class="image">  
<p align="center">  
<img src="https://user-images.githubusercontent.com/122958638/235541512-b097bbf0-9dbf-4847-9026-c4a55faf9203.JPG" width="40%"><br>
</p>
</figure>

<p align="center">
Figure 9.3: Top of Physical Board
</p>

<figure class="image">  
<p align="center">  
<img src="https://user-images.githubusercontent.com/122958638/235541517-1c06997d-dd2a-45f1-82e4-c310ea5e2cd5.JPG" width="40%"><br>
</p>
</figure>

<p align="center">
Figure 9.4: Bottom of Physcial Board
</p>

## Changes for the Future

If the team were to make a second version of the hardware design, one of the changes that could be made to improve it would be to change the 3.3V plane to GND. This wouldn't really change much, except this could possibly reduce noise throughout the system. Another possible improvement would be to connect the SCL and SDA pins of the ADC to the microcontroller. The removal of the connections was intentional, as the plan was to create them manually. This was so when collecting data, the wires could be manually switch to where the team wanted to collect data from. In hindsight, it would have been a better idea to program it accordingly, as the separated wires caused us to have to solder them anyway. This caused problems later on, as whenever they touched, it would short the SDA and SCL connections. Another change that  should have made was changing padstacks of most of the components, as a lot of them were either too large or small for the connections. Putting the capacitors for the regulator closer to it would also help reduce noise throughout the system. Finally, reducing the size of the board by bringing all the components closer to each other. 
