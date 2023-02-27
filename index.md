---
title: Mobile Enviromental Sensing Report
---

HERE IS THE TESTING TO SeE iF the LiNk to other files work
[Block Diagram](block_diagram.md)

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

**Search Results Link:** [Link](https://www.amazon.com/s?k=wind+speed&crid=1VOHJZRICCGJD&sprefix=wind+spee%2Caps%2C146&ref=nb_sb_noss_2)
#### Selected Product
1. [HoldPeak 866B Digital Anemometer Handheld Wind Speed Meter for Measuring Wind Speed, Temperature and Wind Chill](https://www.amazon.com/HOLDPEAK-Anemometer-Measuring-Temperature-Backlight/dp/B00ZHKWCP4/ref=sr_1_4?crid=1VOHJZRICCGJD&keywords=wind%2Bspeed&qid=1673918793&sprefix=wind%2Bspee%2Caps%2C146&sr=8-4&th=1)

* Vendor: HoldPeak/Amazon
* Description: Handheld Wind Speed Meter for Measuring Wind Speed, Temperature and Wind Chill with Backlight and Max/Min
* Price: $30.99

<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/61YqzEkMWCL._AC_SL1500_.jpg" width="30%"><br>  
 </div>
</figure>


**Positive Comments**

| Voice of the customer | Restated customer needs |
|---|---|
|“Having accurate readings of the immediate winds is crucial to adjusting the windage corrections in my hunting scopes or my target sights. Compact and easy to use, it makes the difference between a miss and a well-aimed shot.”|1. The product needs to have accurate readings (explicit) <br> 2. The product is compact and easy to use (explicit). <br> 3. device is good for hunting (latent). |
|“It is the easiest way to test the airflow of my central A/C. I recorded the flow with a new filter to establish a benchmark. Now I can monitor the condition of my filter and if the coils freeze over I will be able to see a decrease in air flow. This meter measures the speed and temperature of the air flow to each room. Easy to read. Highly recommend it as a must have for a homeowner.”|1. The device is good at testing airflow (explicit). <br> 2. Is able to measure the decrease in air flow (explicit). <br> 3. Measures the speed and temperature (explicit). <br> 4. Good for homeowners (explicit).|
|“This little gizmo works well and is more sensitive than I expected. While I was testing one without, a small rock flew from the filter and broke all but one of the fan blades. Only odd setting is the minimum airflow in my opinion. You need air to be moving through already to get an actual reading, which in some circumstances may be difficult if you can't see the screen while testing. Personally I don't need this function, but it is still a nice feature.. Batteries included, 2 AAA.|1. Very sensitive reading (explicit) <br> 2. Needs to be more durable (latent) <br> 3. Has multiple features (latent) <br> 4. Comes with batteries (explicit)|

**Negative Comments**

| Voice of the customer | Restated customer needs |
|---|---|
|“The unit was attractive and simple to use. Unfortunately, its readings had little relation to reality! I received the unit on a 60 degree fahrenheit day, with a strong weather front of 24 mph winds moving through my area. the HOLDPEAK 866B Digital Anemometer insisted it was 72 degrees and through repeated wind measurements gave me an average wind speed of 8 mph with max wind speed of 11.5 mph. I returned the device at a cost of $4.20, despite being a Prime member, because of the lithium batteries that require special hazmat handling.”|The readings need to be accurate (explicit) Requires lithium batteries (explicit)|
|“Neither one agrees with the other in terms of temp and wind speeds. Off by a country mile. The weather apps are showing a temp of 76 and winds at about 18-20 mph. Save your money, these both are truly worthless.”|Readings need to be accurate (latent) Temperature and wind speed need to be correct (explicit)|
|“ Next time we went to use it...all buttons would work...but it wouldn't read the wind. Took it home and pulled the batteries, let it sit a while, got a reading and then...nothing. Changed batteries, got a reading and then...nothing. Fussed with it again a couple days later and got a reading...turned it off and then back on...and...nothing. Just seems to work occasionally when it wants to but not when I need it to. What's the point? I can't trust it to be there when I need it. It was never knocked around, dropped, gotten damp...etc.”|Needs to read correctly every use (explicit) All buttons should function correctly (explicit) Shouldn’t need much maintenance (latent)|
 


#### Search #2
**Keywords:** wifi weather station

**Search Results Link:** [Link](https://www.amazon.com/wifi-weather-station/s?k=wifi+weather+station)

#### Selected Product
2. [Ambient Weather WS-2902 WiFi Smart Weather Station](https://www.amazon.com/Ambient-Weather-WiFi-Station/dp/B01N5TEHLI/ref=sr_1_1_sspa?keywords=wifi+weather+station&qid=1673917945&sr=8-1-spons&ufe=app_do%3Aamzn1.fos.18ed3cb5-28d5-4975-8bc7-93deae8f9840&psc=1&smid=A2ANVX7C75D1I&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUEySE84OTNCSkoxRlpRJmVuY3J5cHRlZElkPUEwNDI4MDU1T0U5MDBLN0taNDNGJmVuY3J5cHRlZEFkSWQ9QTAyNTM4MTkzQ1ZFU1I5TjVXMzZPJndpZGdldE5hbWU9c3BfYXRmJmFjdGlvbj1jbGlja1JlZGlyZWN0JmRvTm90TG9nQ2xpY2s9dHJ1ZQ==)

* Price: $189.99
* Vendor: Ambient Weather Store
* Description: Allows you to monitor your home and backyard weather conditions with brilliant, easy-to-read LCD color display. Wireless all-in-one integrated sensor array measures wind speed/direction, temperature, humidity, rainfall, UV and solar radiation. Supports both imperial and metric units of measure with calibration available. Enhanced Wi-Fi connectability option that enables your station to transmit its data wirelessly to the world's largest personal weather station network.

<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/51fSHzJV5dL._AC_SL1000_.jpg" width="50%"><br>  
</div>
</figure>

**Positive Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“. Rain gage that measures not only the amount of rain but hourly rain fall as well as 24 hour rain fall, weekly, monthly and rain event totals. The unit has a wind vain and anemometer for wind direction and speed, of course. It also has temperature with heat index and wind chill. We have a pool so I love that the unit measures UV index and Solar Radiation. Assembly: Not too difficult. Everything goes together pretty easy if you have a basic knowledge of putting things together. As for the unit itself the wind gauge does not look to read over 99.9 mph.”|1. The product is easy to assemble (explicit). <br> 2. It measures all aspects of weather, even less conventional ones, including UV index and radiation. (latent) <br> 3. The product should work for extreme weather conditions (latent).|
|“The color display is easy on the eyes although its much smaller then the one we had before. Reading the settings from an angle does seem a bit off but that's okay for us. Setting it up to Wifi takes a bit of doing and if you're not computer literate then it could be complicated. Getting the batteries in the unit that goes outside was a bit different, It doesn't clearly show you in the instructions and you'd need to be careful not to brake something. Took about 5 minutes to mount. I would recommend this model…”|1. Nice color display for readings (latent) <br> 2. Easy to set-up via Wi-fi (latent) <br> 3. Easy to install & replace power (explicit)|
|“1. Functional Design. The Ambient Weather station (AW) is the clear winner and way, way ahead of Acurite (AR). For starters, the internet connectivity is built-in and utilizes wireless. That is a horribly outdated and expensive design. Setup with the AW station was a breeze...I was assembled, mounted, and up and running on Wunderground within 20 minutes, and most of that was with the physical assembly. <br> 2. Accuracy. Once again, AW is the clear winner. All the readings on the AW were spot on right out of the box. Temp, rainfall, etc were good with no calibration necessary - though all readings can be calibrated if needed, that functional adjustment is built into the console. <br> 3. Durability. This is the one area I cannot yet commend the AW on, only time will tell. It appears to be a better-built unit so I am optimistic and will update this review as necessary.”| Functional design (explicit) <br> 2. Accurate readings (explicit) <br> 3. No calibration needed (latent) <br> 4. Durable (explicit)|

**Negative Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“Couldn't connect the console to an Android phone, an iPhone, or an iPad. A WiFi connection never worked. The process just kept moving in an endless circle of "reconnect" warnings. <br> The console screen display sucks. Amazon reviewers mention an "upgrade" to the console in the "C" version, to make it more readable. I received the "D" version and the console screen is just barely readable in room light. Any sunlight overwhelms the display.”|1. Needs to be able to easily connect to non-computers (smartphones, tablets). (latent) <br> 2. User interface on app needs to be clear and focused on functionality (latent) <br> 3. Needs console screen bright enough to read in direct sunlight (explicit)|
|“It comes in a million pieces - including extra pieces that apparently do go with the unit? A weird spring? (see pic) See UPDATE below in next item. It took a while, but I found out what it was. It's not in the huge manual. <br> The app is completely useless - I live relatively rurally. So it would not register my address. Instead, I was given a choice to choose someone else's address(es) all more than 30 miles from me for weather checks..  <br> It does NOT come with a post of ANY kind - so purchase one.”|1. Must be easy to assembly - if assembly is required (latent) <br> 2. Needs simple connectivity to smartphone devices. (latent) <br> 3. Needs app that works for rural locations (explicit) <br> 4. Needs to either come with set-up post, or not need one (latent)|
|“The Unit is BROKEN AGAIN. Well yesterday it seems that the outside temperature is now reading 8 to 10 degrees warmer than the surrounding area. But again, a year later, its not working again. It's been stuck at 10% Humidity and I did the reset after removing the batteries and taping up the solar sensor and that didn't work.. I live in a northern climate environment and they are saying "Heat" caused the failure.... Its a WEATHER STATION designed to measure heat... if their equipment is that delicate that it can't stand a little heat then their product is JUNK in my opinion.”|1. Needs to be durable (explicit) <br> 2. Needs to be accurate (latent) <br> 3. Needs to be fast updating (latent)
 
#### Search #3
**Keywords: temperature sensor for outdoor animals**

**Search Results Link:** [Link](https://www.google.com/search?q=temperature+sensor+for+outdoor+animals&rlz=1C1ONGR_enUS965US965&oq=t&aqs=chrome.0.69i59l3j0i67j69i57j69i61j69i60l2.551j0j7&sourceid=chrome&ie=UTF-8)

#### Selected Product
3. [Temp Stick Remote WiFi Temperature & Humidity Sensor](https://www.amazon.com/Wireless-Temperature-Monitoring-Unlimited-Historical/dp/B01HH7YD2Y/ref=sr_1_1?crid=F1KLO4EC7W5H&keywords=temp%2Bstick%2Bremote%2Bwifi&qid=1673921161&s=books&sprefix=temp%2Bstick%2Cstripbooks%2C177&sr=1-1&ufe=app_do%3Aamzn1.fos.18ed3cb5-28d5-4975-8bc7-93deae8f9840&th=1)
* Price: $149
* Vendor:  Ideal Sciences
* Description: 24/7 remote wifi temperature and humidity monitor with detailed data logging.

<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/612SBcK04TL._AC_SL1000_.jpg" width="45%"><br>  
</div>
</figure>

**Positive Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“The units are pretty pricey but when I have high priced meat I can't afford to lose, the cost of the temp stick is well worth it. That being said, it's really great to have a device that will text and email if there is a problem and I have tested the product by taking it out and waiting for my alert and sure enough it worked perfectly. I can look at the device on my phone, tablet and desktop computer and I love that. I would not have anything else..”|1. Automatic electronic updates (explicit) <br> 2. Higher price is worth higher quality product (latent) <br> 3. App and website connected to the sensor (latent)|
|“The Temp Stick is a great investment that alerts when refrigerators and freezers have mechanical issues to allow you to mitigate product loss. The Temp Stick not only keeps me apprised of the freezer temperature, but recently alerted me to a temperature spike, which was the result of a capacitor that failed, allowing me to take quick action to save everything in the freezer until I could procure the right capacitor and make the repair a few days later. <br> Setup and management is easy and the signal is strong -- even through the walls of a stainless steel commercial freezer.”|1. Alerts when temperature rises (explicit) <br> 2. Easy setup and management/ user-friendly (latent) <br> 3. Strong wifi signal for reliability (latent)|
|“It was easy to set up (you need to have WiFi) and worked great. Once it lost connection and couldn't report its readings, but Customer Support quickly got it working again -- there was an issue connecting to my Temp Stick account. The attic is directly above my office where the WiFi router is, so I'm hoping it will have a good connection. I'll update this review after I get some readings from this 2nd Temp Stick. <br> Update (01/02/2023): My new Temp Stick has been running for several days and it works great! It gets a good connection from the attic to the WiFi router in the office below.”|1. Strong customer support (latent) <br> 2. Strong wifi connection (latent) <br> 3. Alerts when area gets too cold (explicit)|

**Negative Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“Update #2: Tried the Temp Stick on a different mobile hotspot device in the phone store & it still WOULD NOT CONNECT. Attempted to connect to Hotspot on cell phone & wouldn't work. I was able to get it to connect to home internet & work, but we need to use it in our camper for our dog- home internet is no good. He said it'd be better to use a mobile Hotspot device so we dropped $$$ on a MiFi mobile hotspot... still can't get the temp stick to connect, but again other devices connect fine. ”|1. Needs to connect to mobile hotspot (explicit) <br> 2. Needs to be suitable for travel (latent) <br> 3. Needs to have strong customer support (latent)|
|“I bought this for a second home in an area where the internet goes out occasionally. When internet service goes out the temperature sensor keeps trying to communicate, and the batteries die. When the internet service is restored, it cannot be reconnected without changing the batteries and sometimes resetting the device. Not convenient when you live far away from your second home. I feel as if I wasted my money.”|1. Needs to rely on power source other than batteries (latent) <br> 2. Needs to be able to reconnect after going offline (explicit) <br> 3. Needs to be convenient for long distances (latent)|
|“I was never able to get the device to connect via their instructions/web browser. It appears this was a used/previously returned item as the plastic packaging was already torn open when I received the item. I immediately reached out to customer support and never received a response back from them. I wanted to support a U.S. based business, but the product and customer support are terrible.”|1. Needs straightforward instructions (explicit) <br> 2. Needs to have strong customer support (latent) <br> 3. Needs to remain online at all times (latent)|

#### Search #4
**Keywords:** “Humidity sensing humidifier”

**Search Results Link:** [Link](https://www.amazon.com/s?k=humidity+sensing+humidifier&crid=1K3729Z32UN15&sprefix=humidity+sensing+humidifier%2Caps%2C120&ref=nb_sb_noss_1)
#### Selected Products
4. [Syvio 2.8L Smart Humidity Sensor](https://www.amazon.com/Humidifiers-Humidity-Essential-Diffuser-Ultrasonic/dp/B0B49MSLWQ/ref=sr_1_5?crid=3J8LRPZ47WY7G&keywords=humidity%2Bsensing%2Bhumidifier&qid=1673918199&sprefix=humidity%2Bsensing%2Bhu%2Caps%2C133&sr=8-5&th=1)

* Price: $49.99
* Vendor: Syvio
* Description: This humidifier can hold up to 2.8L of water, and uses a humidity sensor to prevent over-humidification. This humidifier comes with 3 optional humidity levels, and also acts as an aroma diffuser.

<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/51qAkqH90zL._AC_SL1500_.jpg" width="25%"><br>  
</div>
</figure>

**Positive Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“Large tank size makes refill less frequent, also easy to refill on top. Easy to clean.The unit has warm or cool moisture options. It is solid, does not leak.If you fill up the tank to the top level, the water outlet spring may sometimes get stuck due to bending of the tank bottom under the weight of the water and may give an E2 error (no water in the tank) message and shut down.|1. Should be user friendly. (Explicit) <br> 2. Should provide instructions to prevent possible errors. (Latent) <br> 3. Easy to troubleshoot. (Latent)|“ I purchased it on Amazon a few weeks ago and it worked, that is it produced steam, but the humidity sensor/humidity display did not. I received the unit a few days later, it works 100% and it is a slick unit, small but runs 8 to 10 hours for me on a single fill up and has very easy to use controls on its front surface.”|1. Can be fixed by the user. (Explicit) <br> 2. Works for longer than a few hours. (Latent) <br> 3. Easy to use. (Explicit)|
|“The right size, quiet, easy to refill and finally and most importantly: super easy to clean! Cleaning was always an issue and I ended up buying a new humidifier as it was impossible to access certain areas (mainly the tube from the inside) to clean the built-up mold and mineralization.”|Inside should be easily accessible (Latent) <br> 2. Is small enough to be handheld (Latent) <br> 3.Should be easy to clean if the inside gets dirty. (Latent)|

**Negative Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“Went to kirchen to cook. Came back and it had leaked water all over my dresser and and following its corn to my wall outlet and sparking. It almost caught my home on fire and could have killed me and my family."|1. Is not dangerous to use (Latent) <br> 2. Doesn’t damage any electrical components. (Latent)|
|“Next day...leaked...a LOT and continues to do so after several attempts to figure out why. The remote does not work right. When the humidity is extremely low in my home, the read-out says it's over 90%. Right now it's sitting in a tray in my bathtub so I can catch the water it leaks so I don't waste any more.”|1. Does not waste resources (Explicit) <br> 2. Can sense as intended (Explicit) <br> 3. The product (If user controlled) can be controlled easily. (Explicit)|
|“This is not user friendly. Mine shuts off randomly and I’m constantly getting an error (E2) with an annoying beeping sound. Bought a cheap $20 one that works much better. Don’t waste your money on this!”|1. Should be inexpensive (Explicit) <br> 2. Programmed properly to prevent unnecessary errors. (Latent) <br> 3. Does not produce too much noise. (Explicit)|

#### Search #5

**Keywords:** “Weather Station Wifi”

**Search Results Link:** [Link](https://www.amazon.com/s?k=weather+station+wifi&crid=231KER4S305DB&sprefix=weather+station+wifi%2Caps%2C138&ref=nb_sb_noss_1)
#### Selected Products
5. [Tempest Weather System](https://www.amazon.com/Tempest-Weather-Accurate-Forecasts-Wireless/dp/B0868WY7NY/ref=sxin_15_pa_sp_search_thematic_sspa?content-id=amzn1.sym.14a246c3-7a62-40bf-bdd0-5ac67c2a1913%3Aamzn1.sym.14a246c3-7a62-40bf-bdd0-5ac67c2a1913&crid=231KER4S305DB&cv_ct_cx=weather+station+wifi&keywords=weather+station+wifi&pd_rd_i=B0868WY7NY&pd_rd_r=4961ad94-60b3-4af5-b396-5d67f5f137a2&pd_rd_w=FLkwT&pd_rd_wg=d9Wyv&pf_rd_p=14a246c3-7a62-40bf-bdd0-5ac67c2a1913&pf_rd_r=SSF77S1AE7DJ2CEEQWWH&qid=1673920953&sprefix=weather+station+wifi%2Caps%2C138&sr=1-1-a73d1c8c-2fd2-4f19-aa41-2df022bcb241-spons&psc=1&smid=A3RAYC554RKGF9&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFDWDNIN1c0U1NZMEUmZW5jcnlwdGVkSWQ9QTA5NDQ3ODIzMzlHT1hFSVRPQzQ0JmVuY3J5cHRlZEFkSWQ9QTA0MTg5NTEyQURWTkwxMUNCRThSJndpZGdldE5hbWU9c3Bfc2VhcmNoX3RoZW1hdGljJmFjdGlvbj1jbGlja1JlZGlyZWN0JmRvTm90TG9nQ2xpY2s9dHJ1ZQ==)

* Price: $329.00
* Vendor: WeatherFlow
* Description: The weather system has a built-in wind meter. Rain gauge, light and pressure sensors, as well as being able to detect temperature and humidity

<figure class="image">  
<div style="text-align: center">  
<img src="https://m.media-amazon.com/images/I/31TaKuy4jtL.jpg" width="45%"><br>  
</div>
</figure>

**Positive Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“. I haven't had connectivity loss as frequently (admitted low sample set). <br> Again, I don't have much of a duration to feel confident this was "lucky", but this PWS predicted rain (70% - 80% chance) that actually materialized about 5 days out, when no other app forecasted the rain until 48 hours or less (Weather Channel, etc). Needed to be cleaned out from time to time (leaves, debris stuck in the cup).”|1. Setup is easy. (Explicit) <br> 2. Accurately reads everything it senses. (Explicit) <br> 3. Does not require to be cleaned often. (Latent)|
|“Truly 5 mins to set up. Connection to Alexa is easy (most important feature for me). Durable. T Low profile with no extraneous parts, like vanes.”|1. Device is made from durable materials. (Latent) <br> 2. Has no unneeded parts. (Latent) <br> 3. Wifi connection is easy to do, and requires little setup. (Explicit)|
|“Installation was very easy, but make sure you record the numbers on the device before putting it on a staff up high. Operation has been trouble-free. It’s neat to have all that site data, especially in a rural area where NWS or commercial services are keyed to stations farther away. ”|1. Easy to install (Explicit) <br> 2. Displays data quickly (Latent) <br> 3. Easy for users to operate. (Explicit)

**Negative Comments**

| Voice of the customer | Restated Customer Needs|
|---|---|
|“ 1. It will not charge despite 4-6 hours of direct sun <br> Battery was dead in 2 weeks. <br> 2. It would lose connection with base station after an hour when on external battery despite being 20 feet from hub and router.
I just can not get more than 10 min of data when on battery power, disconnect power and it works but battery dies…”|1. Will charge within a couple hours (Latent) <br> 2. Battery is able to last for at least a few hours (Latent) <br> 3. Should have a strong connection to wifi (Latent)|
|“This thing never had the correct temp wind or rain. There software is a total joke. It sometimes works and sometimes doesn’t.”|1. Device has accurate readings (Explicit) <br> 2. Software is easy to manage/debug. (Latent) <br> 3. Should be under $300 to make it more affordable. (Explicit)|
|“I get wind spikes of 70 mph when heavy rain and strong winds are here. Now my temp and humidity have gone bonkers with a long period of heavy fog has been on going. I am sure the sensor has gotten wet and caused the temp reading to go as low as -37 and slowly creeps up to 57 then back down while humidity is jumping all over the place.”|1. Sensors can perform under harsh weather conditions. (Latent) <br> 2. Humidity does not affect the sensors (Latent) <br> 3. Can connect to wifi during a storm. (Latent)|


 



### Organizing Need Statements
#### Initial Notes

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214115946-484b1696-6e26-4b2a-b59a-5bbf313eea49.png" width="70%"><br>
</div>
</figure>

#### Grouped Notes

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116096-13ec02ca-005a-4afa-b22a-cb1dd1958bc6.png" width="70%"><br>
</div>
</figure>

##### Grouped Notes Key:

|Color:|Meaning:|
|---|---|
|Green|User-friendly/interaction|
|Blue|Durability/hardware|
|Pink|Accuracy/software|
|Yellow|Conveinence/Safety|
|Orange|Needs and Meta Needs|

#### Ranked Notes

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116180-2cc50e3e-7e87-4835-8ff1-bd9542341d74.png" width="70%"><br>
</div>
</figure>

##### Ranked Notes Key:

|Amount of Stars|Amount of importance|
|---|---|
|3 Stars:|Very Important|
|2 Stars:|Important|
|1 Star:|Less Important|

#### Compiled Notes

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116243-0825968d-1118-4126-9046-b9f03bfbf8b6.png" width="70%"><br>
</div>
</figure>

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

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116311-40511671-f01c-4196-bb75-e4e6fbd40425.png" width="70%"><br>
</div>
</figure>

After organizing the ideas, the team started by eliminating movement possibilities that didn’t seem to be the most suitable for the remote weather station. Items that didn’t meet our stakeholders needs were excluded with a primary focus on a lack of accuracy required for functioning. Once there were three categories of specific ideas, the team began to eliminate any potential ideas that wouldn’t coincide with the chosen idea. After compiling all of the ideas, the specified general idea groups would become the three design concepts outlined below.
The rankings as seen in the stars of each major category of needs was chosen based on the device and how important it was to the user for the product to have such requirements.

### Three Chosen Ideas

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116436-f0d1f49a-0f96-4a50-be69-5faf61e4f8c9.png" width="70%"><br>
</div>
</figure>

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214118667-aa4aca19-75c7-42b9-adf9-adaae294bac9.png" width="70%"><br>
</div>
</figure>

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116548-021481ad-4eaa-4471-9d1e-e3ad41df61db.png" width="70%"><br>
</div>
</figure>


### Ranked Ideas

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116605-83a6d0e9-b122-42e4-9baf-28e6624f695a.png" width="70%"><br>
</div>
</figure>

### Design Concepts
The team worked together to come up with the overall design of the three concepts, and with the help of Gavin, Abigail, and Jacob, they sketched each concept.

#### Concept 1

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116697-20563f9f-4f2d-4037-af0d-a69326c82453.png" width="70%"><br>
</div>
</figure>

#### Concept 2

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116756-8b54c61f-10c5-42e8-b3b7-75410e7e72a7.png" width="70%"><br>
</div>
</figure>

#### Concept 3

<figure class="image">  
<div style="text-align: center">  
<img src="https://user-images.githubusercontent.com/122709787/214116804-5879344e-ecd6-46a9-97c6-dc4ecd067f28.png" width="70%"><br>
</div>
</figure>

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

|Name|First Choice Communication|Second Choice Communication|Third Choice Communication|
|---|---|---|---|
|Jacob Pisors|_Discord_|_Verbal_|_Text_|
|Abigail Gordon|_Text Message_|_Verbal_|_Email_|
|Claire Rogers|_Text Message_|_Verbal_|_Discord_|
|Gavin Benvenuto|_Verbal_|_Text Message_|_Discord_|

### Communication Procedures
_Team Communication:_

All team members will conduct communication to one another through group text, in class collaboration and possibly through Zoom as seen in Table 1. Our main choice for communication is either text or verbally.

_Instructor Correspondence:_

Claire Rogers will be responsible for instructor correspondence and will communicate all information to the team via text.

### Meeting Schedule
_Team Prefered Meeting Time:_

As shown above, every point that is highlighted in green represents times that all team members will be available to discuss/work on assignments.. For our team, each of us are available on Friday from noon to 2pm. Therefore we will meet on Friday at noon each week as seen in the above **Table 2**.

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
