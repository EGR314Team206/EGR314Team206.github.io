# Block Diagram
<div align="center">
<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122958638/222036623-96a19ab6-1c92-4ce2-835e-955b76efb84f.png" width="70%"><br>
</div>
</figure>
</div>

<p align="center">
Figure 1: Block Diagram
</p>

Our block diagram demonstrates who has what subsystem, and where each component will be located relative to the PIC18F27Q10. After Microcontroller Selection and Component Selection, we could place what pins every component would be using on the microcontroller. For example, the ESP32 will be using the RX1 and TX1 pins for transmitting data to ad from the microcontroller with the pins RC7 and RC6. The same pins can be used for both I2C modules (RB2, RB3) and the RX2, TX2, and MCLR (RE3, RB7, RB6) pins will be connected to the MPLAB snap for in circuit programming. We plan to have a voltage regulator to maintain a voltage of 3.3V from a 9V input. We will use the 3.3V to power everything except the motor driver, motor, and anemometer. The 9V will be allocated to everything else. 
  
The microcontroller, ESP32, ICSP, and voltage regulator. will be managed by Gavin Benvenuto, the wind sensor and one of the ADC's will be managed by Claire Rogers, the moisture sensor and the other ADC by Jacob Pisors, and the motor/motor driver by Abby Gordon.
