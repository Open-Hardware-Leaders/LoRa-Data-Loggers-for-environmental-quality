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

| Attribute                                    | Value [imperial]         | Value [SI]             |
| ----------                                |:-----:                   | :-------------:        |
| Weight                                    | [lbs]                    | 1 [kg]                 |
| Footprint                                 |  [in]                    | 30x5 [cm]              |
| Battery Capacity                          | 6800 [mAh]               | 6800 [mAh]             |
| Battery Discharge Rate                    |  [A]                     |   [A]                  |
| Nominal Current Draw                      |     [A]                  |     [A]                |
| Operating time                            | 3 [months](continual use)|3[months](continual use)|
| Approximate Max wireless communication    |     []                   | 3 [km]                 |
| Communication (in this guide)             | Arduino IDE (windows, mac, GNU/linux) | |
| Cost                                      | ~ $350                 |                        |

### Features
This data logger is designed to function similarly to the [Cave Pearl Proyect data logger](https://thecavepearlproject.org/category/diy-build-a-pro-mini-logger/) designs:
 * __Rocker-Bogie:__ The Rocker-Bogie suspension system allows all 6 wheels to continually be in contact with the ground while climbing over obstacles
 * __Differential Pivot:__ Allows weight to be mechanically offloaded from one side of the rover to the other while climbing
 * __6-Wheel Ackerman Steering:__ Driving and steering/turning mechanism that governs where the wheels point and how fast each of them will move.

###

### Pathways
* [Survey for scientists](https://drive.google.com/open?id=1LG6TfIyw4GZSVESFRLKz3ml2B999uxwez4n2eBbThyI)
* [Slides introducting the data logger](https://drive.google.com/open?id=1zq_IMxR3ppLNEuhrN3IsdEPZg6zOZ_rIceaL0tdQykI)


## Value Proposition generic for Open Hardware
### The product
An Open source data logger that people can find online, access, replicate, buy and delivers a set of funcionalities, use values with certain quality.

### Pain relievers
I could either buy it, replicate it, build it myself, or order someone else to manufacture it because is not patented.

### Gain creators
The Open source data logger allows to study, and improve its current desing and many people can participate in making it better.  

## The Value proposition (more specific)
### The product
The product proposed is a data logger to assess environmental quality. This product is a small, cheap and low consumption device that allows to measure different variables like freshwater environments. Another important feature about these data loggers will be their connectivity to Lo-Ra Wan technology that will also be connected to the internet. 
This product will bring information at real time about sites of interest 

### Pain relievers
Freshwater environments are recreational places widely used by society. For this kind of use environmental monitoring could tell us if the place is safe. 

### Gain creators
People could be empowered with facts that allows them to make a struggle or any kind of social claim.
State will be able to announce that their remediation politics were effective to make a healthier environment. 
