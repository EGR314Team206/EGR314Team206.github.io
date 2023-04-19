# Hardware Proposal

## Schematic Design
  Our entire system will be powered by 9V batteries that will be connected to every other part of the system that requires power. Our design utilizes a switching voltage regulator dropping from 9V to 3.3V, meaning we will have 2 power rails for the entire system. Most of the system will be powered by the 3.3V such as the mircocontroller, ADC's ESP32, and OLED. However, three of our components will be powered by the 9V power rail such as the voltage regulator, anemometer, motor driver and motor.

## Subsystems

### Microcontroller/Voltage Regulator
  Our microcontroller (PIC18F27Q10) connects to every other system on our board, including our LED array, button with pullup resistor, and ESP32. The ESP32 allows us to connect to wifi. It has 2 SPI and 2 I2C modules which can be used with our motor driver and ADC's. It will be managed by Gavin Benvenuto.

### Wind Sensor
  Our Anemometer can detect wind speed and send it as an analog signal into one or our ADC's (MCP34421T-E/SN_CER). It will convert this into a digital signal which is then sent back to our microcontroller. We can use this to determine the direction of the wind which can be used to determine what direction to turn the sail in. It will be using one of the I2C modules and will be managed by Claire Rogers
  
### Moisture Sensor
  We plan to make a custom moisture sensor for our system, which will send a signal to our second ADC (MCP3426). This will allow us to detect wether or not our system in in water and allow the rest of the system to operate. It will be using one of the I2C modules and be managed by Jacob Pisors
  
### Motor and Motor driver
  Our motor (35L048B1B) and motor driver (IFX9201SG) both operate at 9V and will function based on the information given by the anemometer. We plan to have it turn a sail based on the direction of the wind. It will using an SPI module and will be managed by Abigail Gordon

## Our Schematic design

This shows the first iteration of our full Schematic:
[To Download](https://github.com/EGR314Team206/egr314team206.github.io/files/10857227/SystemDesign.pdf)
