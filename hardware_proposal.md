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
  Our motor (35L048B1B) and motor driver (IFX9201SG) both operat at 9V and function based on the information given by the hall effect sensor. We planned to have it turn a sail based on the direction detected by the hall effect sensor. It used an SPI module and was managed by Abigail Gordon
  
### Meeting User Needs
  We met user need by making a design that could not only detect whether or not the system is within water, but also is able to communicate this information over wifi.

## Our Schematic design

This shows the first iteration of our full Schematic:
[To Download](https://github.com/EGR314Team206/egr314team206.github.io/files/10857227/SystemDesign.pdf)
