Mobile Enviromental Sensing Report
====

ASU EGR-314: Embedded System Design Project II
---------------------------------------------

_Team Member Names:_ 

_Jacob Pisors, Claire Rogers, Gavin Benvenuto, Abby Gordon_

**_Last Updated: 28 Feburary 2023_**

**Dr. Aukes** | **Spring 2023**



# Introduction

Mobile weather stations are important for giving accurate weather information to local populations. These stations can also be used to monitor weather conditions during response operations. As well as personal or specific business needs where control, monitoring, and adaptation under select conditions are required. People need the ability to sense and respond to environmental conditions such as temperature, humidity, atmospheric pressure, wind speed, and other modalities using I2C or SPI for a mobile weather station that connects over Wi-Fi. Throughout this report, the team will discuss different topics related to the completion of a successful prototype.

# Table of Contents

## [Team Organization](team_organization.md)


Our Team Organization briefly covers our Team Charter and Mission Statement. It describes our main goals for this porject as well as what we hope to learn and accomplish. For more information on the team’s establishment please see [Appendix A](Appendix_A.md).

## [User Needs & Benchmarking](user_needs.md)


Our User Needs and Benchmarking introduces how through VOC (Voice of Customer) Benchmarking, we were able to identify common issues addressed with products similar to our design restraints. By observing both positive and negative comments, we could identify what worked, and what was a recurring issue. We later grouped these into serperate categories of type and importance. Inside shows our process step by step, and how we came to identify these needs.

## [Product Requirements](product_requirements.md)


In the Product Requirements section, we took what needs we found from the previous assignment and transformed them into requirements. This allows us to put guidelines on the project that weren't set by the instructor. 

## [Design Ideation](design_ideation.md)


The Design Ideation goes over the process of generating ideas for ideas of the final design. In this section you can see the process of grouping, ranking, and coming up with a rough sketch of what our design should be. We generated three possible designs that could be used for the final product.  

## [Selected Design](selected_design.md)


Selected Design briefly goes over how we came to decide what our final design should be, and why it was chosen. It goes more into depth on how our final design will function.

## [Block Diagram](block_diagram.md)


Our Block Diagram goes over how our microcontroller will recieve and transmit data to all the other components. It also shows how each of the components will be powered and by what. 

## [Component Selection](component_selection.md)


Component Selection describes each component selected and a brief paragraph as to why they were chosen. For more information on Component Selection, please see [Appendix B](Appendix_B.md)

## [Microcontroller Selection](microcontroller_selection.md)


In Microcontroller Selection, it has reasoning on why we chose this microcontroller as well as images of the Surface Mount and  Through-Hole versions. It also links to the products page and its datasheet. For more information on Microcontroller Selection, please see [Appendix C](Appendix_C.md)

## [Hardware Implementation](hardware_proposal.md)


Our Hardware Proposal shows how all of our components connect with one another while explaining wha team member what control over what subsystem. We also have the latest iteration of our board, showing the top, and bottom copper planes. To see the power budget of this system, please see [Appendix D](Appendix_D.md). If you would also like to download a copy of the system design click [here](https://github.com/EGR314Team206/egr314team206.github.io/files/10857227/SystemDesign.pdf). If you would like to download a visual representation of our board click [here](NEEDS PHOTOS).

## [Software Implementation](software_proposal.md)


Our software proposal shows the process in which our code will function, how the system will initialize, and what data is being output. It has images of the state diagrams made and descirbes what the main purpose of each one is. We also show the "skeleton" of our code, and describe waht it does/how it does it.

## Lessons Learned


During this semester, our group ran into many issues. From having to change our microcontroller three times, to choosing components that weren't compatible with our design, and not realizing this much later. However, we were able to apply knowledge learned from the previous semester in EGR 304. We learned the iportance of using different forms of communication between chips (i.e. SPI, I2C, UART, etc.). For example, SPI is faster in communication, but I2C can support multi-masters. We learned the difference between switching and linear regulators. The most important thing we learned would have to be the design process as a whole. After EGR 314, we have experience in every step from conecpt, to design, to application. While we don't have vast knowledge in every step of the design process, EGR 314 gave us an introduction into every aspect, which will aid us in future endeavors.

## Recommendations For Future Students


This process was incredibly difficult, and a lot of mistakes were made along the way that could have bee detrimental had they not been identified early on. Luckily after working through this class we have become more knowledgable, and know what to do, and what not to do, in the future when working on projects in the future. For this reason, we have compiled a list for anyone reading who is interested in on working on their own projects.

- When choosing your microcontroller, make sure it has all the necessary firmware to operate your project. More importantly though, make sure it is in the project requirements. We had to change ours three times due to it not meeting project requirements in some way.
- When choosing passive components, it is highly reccomended to choose ones that have the same pad size. This will prevent you having to create many different padstacks and footprints for your components when designing your PCB.
- Make sure your chosen components can handle the voltage being put into them. For one of our systems, one of the capacitors was rated for a lower voltage than what it was actually using, resulting in a lot of noise.
- Always check the supply voltage of your major components. Also, try to have all of your components on either one of two voltage rails. Since a regulator is required for the course, you have the option of using two different voltages when powering components, but if you accidentally choose a components that can only be powered at a certain voltage, you either have to use a second regulator, or choose a different component. Just try to get it right the first time.
- When choosing components, we recommend using ones with larger pads, as this will make soldering easier for the future. You are given 100 sq cm for your board, you will have enough space for larger components.
- Get accoustomed to using C, as it is the language you will be using for about 97% of the class.
- Attend every class. TA's and the professor will always be here to help, plus these might besome of the only times your entire team can meet up.

We hope that these recommendations help students in the future who are having trouble with designing or the class as a whole. Some of these recommendations would have been good reminders that could have prevented uncessary complications we had experienced during the process.

# Appendices

## [Appendix A: Team Organization](Appendix_A.md)

## [Appendix B: Component Selection Table](Appendix_B.md)

## [Appendix C: Microcontroller Selection](Appendix_C.md)

## [Appendix D: Power Budget](Appendix_D.md)

# Code Repository

**[github](https://github.com/EGR314Team206/egr314team206.github.io)**
