# EcoSen - LoRa Data-Loggers for environmental quality (Español abajo)
Environmental monitoring is essential due to the variety of ways in which it is threatened.
Usually recording environmental variables can be carried out by private data loggers. These devices, due to their high costs, or being of closed design, do not allow us to buy in quantity or build them.
Our proposal consists in the design and development of open hardware data loggers with LoRaWan technology for communication with devices for downloading data. The data loggers will be of two types: aquatic and terrestrial. Aquatics will measure relevant data for the determination of water quality such as turbidity, dissolved oxygen, conductivity and pH. The terrestrial, will measure bee activity variables in hive, biological indicators of environmental quality.
These data loggers are based mainly in the [Cave Pearl Proyect](https://thecavepearlproject.org/), but with adaptations to surface waters.

<img src="Images/image_1.jpg" width="100%">

### Motivation
We want to bring to society the passion for monitoring rivers and lakes. Also with the plus of learning about open electronic projects with possibility of reproduce, modify and customize data loggers. The Open technology that we bring is associated with open data repositories that will make the environmental information accessible to everyone!

### The first steps

To begin recording environmental variables is necessary to develop some abilities measuring these. To do that we are gonna start making a [Coqui conductivity sensor](https://publiclab.org/wiki/coqui) of [Public Lab](https://publiclab.org/) website.
<img src="Images/Coqui.jpg" width="100%">


### Specifications & Technical Attributes

The specific attributes of the data logger you build will depend slightly on the type of sensors you buy for the system. The numbers shown below are for the full version of the data logger that contains exactly the parts that we suggest in our build documents and parts list. Below, you can see which parts could be changed for which spec upgrades.

| Attribute                                   | Value [SI]             |
| ----------                                  | :-------------:        |
| Weight                                    | 1 [kg]                 |
| Footprint                                 | 30x5 [cm]              |
| Battery Capacity                          | 6800 [mAh]             |
| Operating time                            |3[months](continual use)|
| Approximate Max wireless communication    | 3 [km]                 |
| Communication (in this guide)             | Arduino IDE (windows, mac, GNU/linux)  |
| Cost                                      | ~ U$S350                 |  

##### Table of compenents

||Quantity|Value U$S|Link|
|----------------|:-----------------:|------------------|--------------------|
|arduino pro mini
|Arduino mega||||
|sensor de temperatura ds18b20||||
|sensor de turbidez||||
|sensor de pH||||
|sensor de conductividad||||
|sensor de oxígeno disuelto||||
|real time clock||||
|Cargador pilas 18650||||
|portapilas||||
|pilas reacrgables||||
|módulo LoRa||||
|Hermetic case||||
|Insumos varios electrónicos (cables, borneras, estaño, etc.)||||

### Features
This data logger is designed to function similarly to the [Cave Pearl Proyect data logger](https://thecavepearlproject.org/category/diy-build-a-pro-mini-logger/) designs:
 * __Autonomous:__ this data logger has an autonomy of several months
 * __Customisable:__ Allows to choose what sensor you want for your data logger 
 * __Wireless communication:__ Thanks to the LoRa connectivity this device can send a measurements to a server and get access to the information wherever you are. This feature is new to the Cave Pearl Proyect data logger.

We chose a Arduino pro-mini to be the "brain" of this data logger for its versatility, accessibility, simplicity, and ability to add and upgrade your own modifications. Any method with which you can communicate with a arduino pro-mini (bluetooth, WiFi, LoRa, etc) can be added to the data logger to get the information from its. 

<img src="Images/ArduinoLoRa.png" width="100%">
 
[List of components](https://drive.google.com/open?id=1hyrhMyJMDih4w9r664UP0bz__xZFTRils_V-fsFg26g)

### Do you want to contribute to the project?
This project need people interested in contribute in different tasks. In order to collaborate with this project, you will need to have some experience in the following:
 * __Coding arduino microcontrollers:__ Although we are already working in the code for the full data logger, improvements of the code are always necessary the best code possible for the device. 
 * __Electronics:__ This project uses components like sensors, different modules, and batteries. 
 * __Community management:__ We need some expertise in the use of social networks and content production. 

Most of the above are skills that you can learn and pick up fairly quickly from watching videos and doing research on the internet, and throughout the project we try to give supplemental information on some of these as well.  See the build documents for more information.

If you want to contribute please send me an email to: alejobonifacio@gmail.com

## Happy building!!
If you have any questions or run into problems during your build, please search for answers and/or reach out on the [forum](https://create.arduino.cc/projecthub/alejobonifacio/ecosen-lora-data-loggers-for-environmental-quality-9dffba).

### Model of README
This README document is based in the NASA Open Source Rover [project](https://github.com/nasa-jpl/open-source-rover) 
