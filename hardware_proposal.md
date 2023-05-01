# Hardware Proposal

## Schematic Design
  Our entire system is powered by 9V batteries that are connected to every other part of the system that requires power. Our design utilizes a switching voltage regulator that regulates voltage from 9V to 3.3V, meaning we have 2 power rails for the entire system. Most of the system is powered by the 3.3V such as the microcontroller, ADC, ESP32, hall effect sensor and OLED. However, three of our components will be powered by the 9V power rail such as the voltage regulator, motor driver and motor.

## Subsystems

### Microcontroller/Voltage Regulator
  Our microcontroller (PIC18F27Q10) connects to every other system on our board, including our LED array, button with pullup resistor, and ESP32. The ESP32 allows us to send data to the MQTT server. It has 2 MSSP communication lines that can communicate with SPI or I2C components. These were used to communicate with the hall effect sensor, moisture sensor and motor driver.
  
### Hall Effect Sensor
  Our Hall Effect Sensor can detect the angle of certain components and communicate with the microcontroller directly. We can use this to determine the angle of certain items. It used one of the I2C modules and was managed by Claire Rogers
  
### Moisture Sensor
  We made a custom moisture sensor for our system, which consists of two wires that hand off the board. While in water, one can be powered by the other. This information is sent to our ADC (MCP3426). This allows us to detect wether or not our system in in water. It used one of the I2C communication lines was managed by Jacob Pisors
  
### Motor and Motor driver
  Our motor and motor driver (IFX9201SG) both operat at 9V and function based on the information given by the hall effect sensor. We planned to have it turn a sail based on the direction detected by the hall effect sensor. It used an SPI module and was managed by Abigail Gordon
  
### Meeting User Needs
  We met user need by making a design that could not only detect whether or not the system is within water, but also is able to communicate this information over wifi.

## Our Schematic design

This shows the first iteration of our full Schematic:
[To Download](https://github.com/EGR314Team206/egr314team206.github.io/blob/main/SystemDesign_Sch.pdf)

## Photos of Board Design
![Screenshot (225)](https://user-images.githubusercontent.com/122958638/235537237-46c90512-1312-446d-a984-f975acc3401e.png)
![Screenshot (226)](https://user-images.githubusercontent.com/122958638/235537241-1025c928-b6d2-43a6-a65f-c604dcdc2c58.png)

## Photos of Physical Board
![XCVC4426](https://user-images.githubusercontent.com/122958638/235541512-b097bbf0-9dbf-4847-9026-c4a55faf9203.JPG)
![EQML7492](https://user-images.githubusercontent.com/122958638/235541517-1c06997d-dd2a-45f1-82e4-c310ea5e2cd5.JPG)

## Changes for the Future

If we were to make a second version of our hardware design, one of the changes that could be made to improve it would be to change the 3.3V plane to GND. This wouldn't really change much, except this could possibly reduce noise throughout the system. Another possible improvement would be to connect the SCL and SDA pins of the ADCs to the microcontroller. The removal of the connections was intentional, as the plan was to create them manually. This was so when collecting data, we could manually switch the wires to where we wanted to collect data from. In hindsight, it would have been a better idea to program it accordingly, as the separated wires caused us to have to solder them anyway. This caused problems later on, as whenever they touched, it would short the SDA and SCL connections. Another change we should have made was changing padstacks of most of the components, as a lot of them were either too large or small for the connections. Putting the capacitors for the regulator closer to it would also help reduce noise throughout the system. Finally, I would reduce the size of the board by bringing all the components closer to each other. 
