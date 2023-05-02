Mobile Environmental Sensing Report
====

ASU EGR-314: Embedded System Design Project II
---------------------------------------------

_Team Member Names:_ 

_Jacob Pisors, Claire Rogers, Gavin Benvenuto, Abby Gordon_

**_Last Updated: 1 May 2023_**

**Dr. Aukes** | **Spring 2023**



# Introduction

Mobile weather stations are important for giving accurate weather information to local populations. These stations can also be used to monitor weather conditions during response operations. As well as for personal or specific businesses that need to control, monitor, and adapt to select conditions. People need the ability to sense and respond to environmental conditions such as temperature, humidity, atmospheric pressure, wind speed, and other modalities using I2C or SPI for a mobile weather station that connects over Wi-Fi. Throughout this report, the team will discuss different topics related to the completion of a successful prototype.

# Table of Contents

## [Team Organization](team_organization.md)


Our Team Organization briefly covers our Team Charter and Mission Statement. It describes our main goals for this project as well as what we hope to learn and accomplish.

## [User Needs & Benchmarking](user_needs.md)


Our User Needs and Benchmarking introduces how through VOC (Voice of Customer) Benchmarking, we were able to identify common issues addressed with products similar to our design restraints. By observing both positive and negative comments, we could identify what worked and what was a recurring issue. We later grouped these into separate categories of type and importance. Inside shows our process step by step, and how we came to identify these needs.

## [Product Requirements](product_requirements.md)


In the Product Requirements section, the team took what user needs were found from the previous assignment and transformed them into requirements. This allowed the team to put guidelines on the project that were not set by the instructor. 

## [Design Ideation](design_ideation.md)


The Design Ideation highlights the process of generating ideas for the final design. In this section, one can observe the process of grouping, ranking, and creating a rough sketch of what the design would look like. Three possible designs were created that could be used for the final product.  

## [Selected Design](selected_design.md)


Selected Design briefly goes over how the team arrived at the final design and why it was chosen. It goes more into depth on how the final design will function.

## [Block Diagram](block_diagram.md)


The Block Diagram goes over how the microcontroller will receive and transmit data to all the other components. It also shows how each of the components will be powered. 

## [Component Selection](component_selection.md)


Component Selection describes each component selected and a brief paragraph as to why they were chosen. For more information on Component Selection, please see [Appendix B](Appendix_B.md)

## [Microcontroller Selection](microcontroller_selection.md)


In Microcontroller Selection, reasons are given as to why the team chose that specific microcontroller as well as images of the surface mount and through-hole versions. It also links to the products page and its datasheet. For more information on Microcontroller Selection, please see [Appendix C](Appendix_C.md)

## [Hardware Implementation](hardware_proposal.md)


Our Hardware Implementation shows how all of the components connect with one another while explaining what team member had control over what subsystem. The latest iteration of the PCB is shown including the top and bottom. To see the power budget of this system, please see [Appendix D](Appendix_D.md). To download a copy of the system design click [here](https://github.com/EGR314Team206/egr314team206.github.io/files/10857227/SystemDesign.pdf).

## [Software Implementation](software_proposal.md)


Software Implementation explains how the code will function, how the system will initialize, and what data is being outputted. Images of the state diagrams are also included with a description of each one. The "skeleton" of our code is provided and what it does.

## Lessons Learned


During this semester, our group ran into many issues. From having to change our microcontroller three times, to choosing components that weren't compatible with our design, and not realizing this until much later. However, the team was able to apply knowledge learned from the previous semester in EGR 304. We learned the importance of using different forms of communication between chips (i.e. SPI, I2C, UART, etc.). For example, SPI is faster in communication, but I2C can support multi-masters. The team also learned the difference between switching and linear regulators. The most important thing learned was the design process as a whole. After EGR 314, the team has experience in every step from concept, to design, to application. While the team does not have vast knowledge in every step of the design process, EGR 314 gave us an introduction into every aspect, which will aid us in future endeavors.

## Recommendations For Future Students


This process was incredibly difficult, and a lot of mistakes were made along the way that could have been detrimental had they not been identified early on. Luckily after working through this class the team has become more knowledgeable, and know what to do, and what not to do, in the future when working on projects. For this reason, we have compiled a list for anyone reading who is interested in working on their own projects.

- When choosing the microcontroller, make sure it has all the necessary firmware to operate your project. More importantly though, make sure it is in the project requirements. The team had to change three times due to it not meeting project requirements in some way.
- When choosing passive components, it is highly reccommended to choose ones that have the same pad size. This will prevent you having to create many different padstacks and footprints for your components when designing the PCB.
- Make sure the chosen components can handle the voltage being put into them. For one of our systems, one of the capacitors was rated for a lower voltage than what it was actually using, resulting in a lot of noise.
- Always check the supply voltage of the major components. Also, try to have all of the components on either one of two voltage rails. Since a regulator is required for the course, there is the option of using two different voltages when powering components, but if a component chosen can only be powered at a certain voltage, one either have to use a second regulator, or choose a different component. Just try to get it right the first time.
- When choosing components, pick ones with larger pads, as this will make soldering easier for the future. Given 100 sq cm for the board is enough space for larger components.
- Get accustomed to using C, as it is the language used for about 97% of the class.
- Attend every class. TA's and the professor will always be here to help, plus these might be some of the only times your entire team can meet up.

Hopefully these recommendations help students in the future who are having trouble with designing or the class as a whole. Some of these recommendations would have been good reminders that could have prevented unncessary complications during the process.

# Appendices

## [Appendix A: Team Organization](Appendix_A.md)

## [Appendix B: Component Selection Table](Appendix_B.md)

## [Appendix C: Microcontroller Selection](Appendix_C.md)

## [Appendix D: Power Budget](Appendix_D.md)

## [Appendix E: Bill of Materials](Appendix_E.md)

## [Appendix F: System Verification Table](Appendix_F.md)

## [Appendix G: Topic Table](Appendix_G.md)

## [Appendix H: MPLAB X IDE Setup](Appendix_H.md)

# Code Repository

**[github](https://github.com/EGR314Team206/TeamCode)**
