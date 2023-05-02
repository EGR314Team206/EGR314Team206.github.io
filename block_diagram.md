# Block Diagram
<div align="center">
<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122958638/234701794-8344657e-43d8-4449-bb5d-bbc972b2a1ce.png" width="70%"><br>
</div>
</figure>
</div>

<p align="center">
Figure 1: Block Diagram
</p>

The block diagram demonstrates who completed each subsystem, and where each component will be located relative to the PIC18F27Q10. After Microcontroller Selection and Component Selection, the team could place what pins every component would be using on the microcontroller. For example, the ESP32 used the RX1 and TX1 pins for transmitting data to and from the microcontroller with the pins RC7 and RC6. The same pins can be used for both I2C modules (RB2, RB1). The MCLR, serial programming clock and data pins (RE3, RB7, RB6) were connected to the MPLAB snap for in circuit programming. A voltage regulator was used to maintain a voltage of 3.3V from a 9V input. The 3.3V powered everything except the motor driver, and the motor. 
  
The microcontroller, ESP32, ICSP, and voltage regulator, was managed by Gavin Benvenuto, the hall effect sensor was managed by Claire Rogers, the moisture sensor and the ADC by Jacob Pisors, and the motor/motor driver by Abby Gordon.
