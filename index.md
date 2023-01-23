---
title: Mobile Enviromental Sensing Report
---

# Mobile Enviromental Sensing Report
**Team 206**

_Team Member Names:_ 

_Jacob Pisors, Claire Rogers, Gavin Benvenuto, Abby Gordon_

**_23 January 2023_**

**ASU EGR-314: Embedded System Design Project II**

**Dr. Aukes**

**Spring 2023**

## Introduction

Mobile weather stations are important for giving accurate weather information to local populations. These stations can also be used to monitor weather conditions during response operations. As well as personal or specific business needs where control, monitoring, and adaptation under select conditions are required. People need the ability to sense and respond to environmental conditions such as temperature, humidity, atmospheric pressure, wind speed, and other modalities using I2C or SPI for a mobile weather station that connects over Wi-Fi. Throughout this report, the team will discuss different topics related to the completion of a successful prototype.

## Team Establishment
### Charter
Based on the goals listed in **Appendix A** and through a team discussion, we constructed the following charter:

_Our team will work together respectively and considerately, valuing each other’s input and keeping deadlines and assignment requirements in mind._

### Mission Statement
Based on the project description and project requirements, the team has come up with the following mission statement:

_To be successful in our understanding of embedded design concepts in relation to environmental sensing and their application to the final product, our team will focus on expanding our knowledge of MPLAB X IDE to broaden our interests and discover new areas of curiosity, while ultimately working towards the creation of an interesting, engaging, and educational final product._

In order to accomplish this, the team needs an understanding of environmental sensing and how these concepts can be used to help detect changes in temperature, humidity, pressure, and wind. As well as sharpening our skills in MPLAB X IDE to better understand a different interface and controller. 

For more information on the team’s establishment please see section Appendix A.
## User Needs Benchmarking
### VOC Introduction:
To determine common user needs for devices using sensors for various weather conditions, material of the product, objects with motor control, etc. The team started with searching for  different products that were similar to the requirements given for the project. Keywords used commonly pertained to weather as well as connectivity to find alike products. From there a specific product would be chosen (normally one with many reviews), and  three positive and three negative reviews were taken from it to spot the needs associated with it. Five products were chosen in total for this, and from that, 100 user needs were observed. Listed below are the five products, keywords used to find them, the link for the search results and the product, price, vendor, description, reviews, and a picture of the product chosen.

### Benchmarking:

#### Search #1
**Keywords: wind speed**

**Search Results Link: Link**
#### Selected Product
1. HoldPeak 866B Digital Anemometer Handheld Wind Speed Meter for Measuring Wind Speed, Temperature and Wind Chill
<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/61YqzEkMWCL._AC_SL1500_.jpg" width="30%"><br>  
 </div>
</figure>

* Vendor: HoldPeak/Amazon
* Description: Handheld Wind Speed Meter for Measuring Wind Speed, Temperature and Wind Chill with Backlight and Max/Min
* Price: $30.99

**Positive Comments**

| Voice of the customer | Restated Customer Needs |
|---|---|
|“Having accurate readings of the immediate winds is crucial to adjusting the windage corrections in my hunting scopes or my target sights. Compact and easy to use, it makes the difference between a miss and a well-aimed shot.”|The product needs to have accurate readings (explicit). The product is compact and easy to use (explicit). device is good for hunting (latent). |
|“It is the easiest way to test the airflow of my central A/C. I recorded the flow with a new filter to establish a benchmark. Now I can monitor the condition of my filter and if the coils freeze over I will be able to see a decrease in air flow. This meter measures the speed and temperature of the air flow to each room. Easy to read. Highly recommend it as a must have for a homeowner.”|The device is good at testing airflow (explicit). Is able to measure the decrease in air flow (explicit). Measures the speed and temperature (explicit). Good for homeowners (explicit).|
|“This little gizmo works well and is more sensitive than I expected. While I was testing one without, a small rock flew from the filter and broke all but one of the fan blades. Only odd setting is the minimum airflow in my opinion. You need air to be moving through already to get an actual reading, which in some circumstances may be difficult if you can't see the screen while testing. Personally I don't need this function, but it is still a nice feature.. Batteries included, 2 AAA.|Very sensitive reading (explicit) Needs to be more durable (latent) Has multiple features (latent) Comes with batteries (explicit)|

**Negative Comments
#### Search #2
**Keywords: wifi weather station**

**Search Results Link: Link**
#### Selected Product
2. Ambient Weather WS-2902 WiFi Smart Weather Station
<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/51fSHzJV5dL._AC_SL1000_.jpg" width="50%"><br>  
</div>
</figure>

| Voice of the customer | Restated Customer Needs|
|---|---|


* Price: $189.99
* Vendor: Ambient Weather Store
* Description: Allows you to monitor your home and backyard weather conditions with brilliant, easy-to-read LCD color display. Wireless all-in-one integrated sensor array measures wind speed/direction, temperature, humidity, rainfall, UV and solar radiation. Supports both imperial and metric units of measure with calibration available. Enhanced Wi-Fi connectability option that enables your station to transmit its data wirelessly to the world's largest personal weather station network.
#### Search #3
**Keywords: temperature sensor for outdoor animals**

Search Results Link: Link
#### Selected Product
3. Temp Stick Remote WiFi Temperature & Humidity Sensor
<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/612SBcK04TL._AC_SL1000_.jpg" width="45%"><br>  
</div>
</figure>

* Price: $149
* Vendor:  Ideal Sciences
* Description: 24/7 remote wifi temperature and humidity monitor with detailed data logging.
#### Search #4
Keywords: “Humidity sensing humidifier”

Search Results Link: Link
#### Selected Products
4. Syvio 2.8L Smart Humidity Sensor
<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/51qAkqH90zL._AC_SL1500_.jpg" width="25%"><br>  
</div>
</figure>

* Price: $49.99
* Vendor: Syvio
* Description: This humidifier can hold up to 2.8L of water, and uses a humidity sensor to prevent over-humidification. This humidifier comes with 3 optional humidity levels, and also acts as an aroma diffuser.
#### Search #5
Keywords: “Weather Station Wifi”

Search Results Link: Link
#### Selected Products
5. Tempest Weather System
<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/31TaKuy4jtL.jpg" width="45%"><br>  
</div>
</figure>

* Price: $329.00
* Vendor: WeatherFlow
* Description: The weather system has a built-in wind meter. Rain gauge, light and pressure sensors, as well as being able to detect temperature and humidity.
### Organizing Need Statements
#### Initial Notes
#### Grouped Notes
##### Grouped Notes Key:
#### Ranked Notes
##### Ranked Notes Key:
#### Compiled Notes
### Assessment of User Needs:
The process of forming the user needs statements started with the benchmarking assignment which helped the team understand what consumers expected out of their product and what they thought the product needed improvement on. The team took the positive and negative comments and turned them into user needs. Once the user needs were made, they were separated into groups based on the description. The groups became accuracy, durability, usability/user interaction, and convenience/safety. Safety included all those that revolved around how the product would mitigate harm to the user. Accuracy referred to how the user would interact with the product. Quality dealt with using durable materials to prevent the need to replace parts. The instructions category was for documentation on the item to avoid facilitator or user error. These 5 categories seemed to encapsulate most aspects of the user needs based on the benchmarking process. 
### Weighting of User Needs:
After that was the ranking process, this was a discussion on what was deemed the most important and least important to the project design. Durability, and user engagement deserved three stars, accuracy deserved two stars, and convenience/safely deserved one star. Durability and user engagement/experience were three stars because those were highlighted the most in the benchmarking. The accuracy deserved two stars is not as essential as the above groups. The convenience/safety were 1 star because it is not as important as the other categories since it is not a hazardous product and most customers purchasing this product expect some setup. Overall, the user needs process was very useful in helping the understanding of what the customers wanted. 
## Product Requirements
### Objectives
The goal of this project is to plan, design, and develop a mobile weather sensing station with a motorized control response to show off to companies, professionals, and peers. As well as create a GitHub website for personal portfolios to demonstrate application of embedded systems to future prospects.
### Stakeholders
#### Users:
Rural Dwellers - Those in remote locations may not have accurate weather forecasts or data. With this mobile weather station device, they can respond accordingly to accurate data. Or have an automatic system to do so.

Miners - Those in harsh working industrial environments need to keep workers safe from high pollution, heatstroke, and humidity.
#### Use Cases
_Use Case 1:_ 

34-year-old Steven works as an engineer at WeatherFlow. This year he decided to attend the Innovation Showcase at ASU to review some of the products some of the students have made. He heard that the main focus of the devices was sensing various changes of weather, such as temperature, humidity, and wind speed. Steven is looking for products that can use these variables, and display them on his phone. He is looking to hire some bright, inventive designers that could help improve the products they make.

_Use Case 2:_ 

56-year-old John is a farmer who is used to using various sensors to detect changes in weather. However, he's never known how these sensors work. He’s heard a couple things such as the differences between serial and analog sensors, but he’s never actually known what they meant. He heard that ASUs Innovation Showcase has products that fit this exact description. So, he decided to attend it this year to get a little more insight as to how the equipment he commonly uses works. 
### Converting Use Needs into Specifications
Below are the design aspects which our team derived from benchmarking and  user needs. After compiling and ranking the user needs, inspiration was drawn from categories and simplified into the various design aspects below. The top ranked user needs with the highest frequency would become product requirements.
### Design Aspects
#### 1. Hardware/Product Design
1.1 - The device shall include at least 1 motor/linear actuator with bidirectional control ability using serial-based (I2C or SPI) motor control

1.2 - The device’s size shall be handheld

1.3 - The device’s weight shall be less than 10lbs

1.4 - The materials for the device shall be durable and be able to withstand constant use

1.5 - The device shall allow for high user interaction through the multiple functions

1.6 -  The device shall be designed to prevent damage from valuable/fragile components

1.7 - The device hardware material shall be durable and be able to withstand minor impacts and high levels of interaction (lifecycle of at least one year)

1.8 - The device design shall allow for easy repair

#### 2. Software/Functionality
2.1 - The project ECAD software shall be Cadence

2.2 - The project shall include at least one switching voltage regulator

2.3 - The system logic-level voltage shall be 3.3V

2.4 - The project shall include at At least 2 serial sensors and one serial actuator using SPI or I2C.

2.5 - The project shall include at least one example each of UART, SPI, and I2C.

2.6 - The project shall use the 8 or 16-bit Microchip PIC families & ESP32.

2.7 - The maximum board dimensions shall be 100x100mm.

#### 3. Interactivity & User Experience
3.1 - The device shall work right away without much input from the user.

3.2 - The device shall seamlessly connect to the microcontroller.

3.3 - The device’s user interface shall be intuitive to all users.

3.4 - The device shall include multiple reading points to sense multiple environmental conditions.

#### 4. Customization
4.1 - The device should allow space for integration into the user’s environment.

4.2 - The device should be adaptable to a wide variety of situations.

#### 5. Manufacturing
5.1 - The maximum project budget is $60 per team member.

5.2 - The position of the components shall not change after assembly.

5.3 - The device shall be designed to consist of the least amount of parts possible.

5.4 - The device shall be designed and created to allow for easy maintenance and use accessibility.

#### 6. Safety
6.1 - The device shall have no sharp edges.

6.2 - The device shall have low energy requirements of 3.3 V to prevent risk.

6.3 - Handheld and lightweight to ensure safety.

6.4 - Functionality must be safe to use for one with no technical knowledge. 

6.5 - Any tools used to modify the device must not require a power supply.

### Open Questions
* How can we design a product that is engaging and attracts attendants at the innovation showcase?
* How would the wifi element be incorporated into our weather sensing design?
* How can we use temperature/humidity sensing technology to solve a problem in our community?
* Can we prioritize safety while still creating a product design that fits all other user needs? 
* Will there be room to expand upon our design once it is finished?
* What elements can we include that would set our product apart from anything like it already on the market?
* In what ways can we incorporate a motor into a temperature/humidity sensor design?
* How will the device utilize all project requirements while still being unique from other class designs? 

### Assessing Designs
To ensure designs meet the criteria above, they must be assessed. The manner in which they will be assessed is each design aspect category being weighted as follows: 30%: Durability/hardware, 30%: Usability/user interaction, 25%: Accuracy, and 15%: convenience/safety. Then, each sub-aspect will be assessed by each team member on completion on a scale of 1-3, where 1 is failure, 2 is partial success, and 3 is success. Upon averaging each team member's decisions the design assessment will be finished. At this point, design changes and adaptations will be discussed to increase the score of a design if the team chooses. This will ensure the final product meets requirements.

### Milestones
Design Ideation: 1/20/2023

Team Checkpoint 1: 1/23/2023

Block Diagram: 1/30/2023

Microcontroller Selection: 2/8/2023

Software Proposal: 2/15/2023

Hardware Proposal: 2/22/2023

Team System Prototype Initial Deadline: 3/17/2023

Hardware Implementation: 3/24/2023

Team System Prototype Final Deadline: 3/24/2023

System Verification Part 1: 4/3/2023

Software Implementation: 4/19/2023

System Verification Final Deadline: 4/24/2023

## Design Ideation
To maximize the possible design concepts for the mobile weather station, over one hundred different ideas were brainstormed that covered possible movement, material, and electrical components. The team first began by thinking of different ways in which the sensors could be used, and created ideas off that. Then the team dived into research of what needs user’s have with similar devices.

### 100+ Generated Ideas
After organizing the ideas, the team started by eliminating movement possibilities that didn’t seem to be the most suitable for the remote weather station. Items that didn’t meet our stakeholders needs were excluded with a primary focus on a lack of accuracy required for functioning. Once there were three categories of specific ideas, the team began to eliminate any potential ideas that wouldn’t coincide with the chosen idea. After compiling all of the ideas, the specified general idea groups would become the three design concepts outlined below.
The rankings as seen in the stars of each major category of needs was chosen based on the device and how important it was to the user for the product to have such requirements.

### Three Chosen Ideas
### Ranked Ideas
### Design Concepts
The team worked together to come up with the overall design of the three concepts, and with the help of Gavin, Abigail, and Jacob, they sketched each concept.

#### Concept 1
#### Concept 2
#### Concept 3
## Appendix A: Team Organization
To go back to the “Team Establishment” section please click here.

_Goals:_

* Meet all deadlines & Project Requirements for this course
* Work well and communicate as a team
* Being able to network with field professionals/researchers
* Increase understanding of MPLAB X IDE
* Exploring new areas of possible interest
* Developing a great addition to our engineering portfolios
* Creating an engaging project that attracts field professionals at the innovation showcase

### Communication Channels
### Communication Procedures
_Team Communication:_

All team members will conduct communication to one another through group text, in class collaboration and possibly through Zoom as seen in Table 1. Our main choice for communication is either text or verbally.

_Instructor Correspondence:_

Claire Rogers will be responsible for instructor correspondence and will communicate all information to the team via text.

### Meeting Schedule
_Team Prefered Meeting Time:_

As shown above, every point that is highlighted in green represents times that all team members will be available to discuss/work on assignments.. For our team, each of us are available on Friday from noon to 2pm. Therefore we will meet on Friday at noon each week as seen in the above Table 2.

### Meeting Coordination
_Team Meeting Reminder:_

In order to remind our team about meeting, we will text in our shared group chat a few hours before the meeting begins. If someone is late, we will remind them through text or a call to ensure everyone shows up.

_Team Meeting Changes:_

If there needs to be a change to a meeting, the team member must notify the group and suggest a time they can meet instead. If that time works for everybody, then the meeting will be changed to accommodate.

_Team Preferred Meeting Format:_

Meeting face to face will be the most effective method of communication for our team, however virtual meeting is currently also acceptable. In the future, it will become necessary to have in-person meetings as the course becomes almost exclusively hands-on as it progresses.

_Team Procedures:_

Talk about assignments as a group in class, splitting the work as necessary and then reconvening when the assignment is 90% completed to discuss any questions and make sure everyone is on the same page before submitting.

### Team Coordination
_Team Assignment Submission:_

One member of the team will be in charge of submitting the assignment and must verify with all team members before submitting. 

_Team Knowledge/Skills:_

Each team member will be responsible for a certain part of each assignment. If he or she is unable to complete their part, they must ask for assistance from another member of the team before the due date. This will help catch all members up to speed with the development of the project.

_Team Prefered Design Feedback:_

Each member will check the other team members’ work and cross check it with the feedback given to ensure that it has been acted upon. This will ensure that none of the work produced is conflicting with each other.

### Team Accountability
_Accountability Charter:_

Each team member will be responsible for an equal amount of the work in order to maintain equal responsibility amongst one another. Regular team check-ins will make sure that contributions will not be missed.
 
_Accountability Expectations:_

Each team member will be expected to complete their work in order to be a successful team. We all want to create the best design in the class and that will only be accomplished through unified group work.

_Recognizing Underperforming Team members:_

If they are asking a lot of questions or need a more than usual amount of help to perform a specific task.

_Supporting Team Members:_

We can help each other improve partly during class if it is a brief problem or during our weekly meetings.

### Conflict and Resolution
Controversy can be normal, but we all want to learn and should always be kind and respectful to one another. I don’t believe that this will be an issue in our group, but if it does become a problem, we will host a team meeting to discuss with all the team members to come up with a compromise or resolution for the conflict. 
