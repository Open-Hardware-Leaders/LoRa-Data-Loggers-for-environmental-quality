# EcoSen - Registradores de datos abiertos (o lo más abiertos posibles) para variables ambientales (English below)
El monitoreo ambiental es esencial para el cuidado del ambiente. Particularmente, me interesa poder monitorear ambientes acuáticos. Para medir estas variables una opción son los registradoresd e datos privativos. Estos debido a sus altos costos, o por ser de diseños cerrados nos imposibilitan compararlo o repararlos.
Nuestra propuesta consiste en el diseño y desarrollo de registradores de datos (RD) con tecnologías inalámbricas para tener información en tiempo real en cualquier dispositivo conectado a internet. Los RD pueden ser tanto acuáticos como terrestres. Los acuáticos se espera puedan medir información relevante para el cálculo de índices de calidad de agua ([Pesce y Wunderlin, 2000](https://www.sciencedirect.com/science/article/pii/S0043135400000361)), como ser turbidez, oxígeno disuelto, conductividad y pH. El terrestre va a medir aquellas variables relevantes para la calidad del aire o suelo. 
La base técnica para la construcción de estos registradores es la presente en el increíble proyecto [Cave Pearl Proyect](https://thecavepearlproject.org/), pero adaptandolo a aguas superficiales.

<img src="Images/image_1.jpg" width="100%">

### Descargo de responsabilidad
Este proyecto se encuentra en gestación por lo que vamos a ver es su evolución. Aún no hemos logrado un perfecto funcionamiento de lo propuesto ni con todo tipo de sensores ni con la conectividad inalámbrica, así que cualquier persona que se quiera sumar es bienvenida. Puedes comuncarte con alejo.bonifacio@unc.edu.ar

## Motivación
Queremos traer a la sociedad la pasión por el monitoreo de ríos, lagunas, lagos y todo tipo de humedales. Además, reconocemos la importacia de aprender acerca de aprender acerca de proyectos de electronica abierta con la posibilidad de reproducir, modificar y personalizar los RD. La tecnología abierta que queremos compartir es asociada a repositorios que harán de la información accesible a cualquier persona. Si en algún momento crees que alguna información no es lo suficiente pública por favor nos lo haces saber.

## Primeros pasos
[// ### The first steps, measuring
To begin recording environmental variables is necessary to develop some abilities measuring these. To do that we are gonna start making a [Coqui conductivity sensor](https://publiclab.org/wiki/coqui) of [Public Lab](https://publiclab.org/) website.
<img src="Images/Coqui.jpg" width="100%">
With this task, we are learning to measure environmental variables with an open source hardware
]

### Second step, logging
To begin logging we are going to made an Arduino Uno based data logger. This data logger is based in one of the [Cave Pearl Projects] (https://thecavepearlproject.org/2015/12/22/arduino-uno-based-data-logger-with-no-soldering/). After complete the datalogger we are going to add a DHT11 temperature and relative humidity module to pin 8 of Arduino Uno. The code.ino is downloadable in the following [link](https://drive.google.com/open?id=17P1dIhY--dl7_n6sXm4gY56F4k5InGaj)or in the Codes folder.
<img src="Images/HumTeDL.jpg" width="100%">


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
|arduino pro mini|1|3.881656805|[->](https://articulo.mercadolibre.com.ar/MLA-643647762-arduino-pro-mini-33v-8mhz-robotica-atmel-atmega328-mona-_JM)|
|Arduino mega|1|9.349112426|[](https://articulo.mercadolibre.com.ar/MLA-621290099-arduino-uno-r3-atmega16u-atmega328-atmel-robotica-todomicr-_JM?quantity=1#position=9&type=item&tracking_id=982584cd-6e84-467d-a826-ffea1fc20edd)|
|temperature sensor ds18b20|1|4.130177515|[](https://articulo.mercadolibre.com.ar/MLA-818621568-sensor-digital-temperatura-ds18b20-cable-sumergible-3-metros-_JM)|
|sensor de turbidez|1|15.66863905|[](https://articulo.mercadolibre.com.ar/MLA-668633063-modulo-sensor-de-turbidez-analogico-liquid-particles-_JM)|
|pH sensor|1|29.5|[](https://www.dfrobot.com/product-1025.html)|
|conductivity sensor|1|79.9|[](https://www.dfrobot.com/product-1797.html?search=conductivity&description=true)|
|disolved oxygen sensor|1|169|[](https://www.dfrobot.com/product-1628.html)|
|real time clock|1|2.970414201|[](https://articulo.mercadolibre.com.ar/MLA-617370292-reloj-tiempo-real-rtc-ds3231-eeprom-24c32-arduino-mona-_JM)|
|18650 battery charger |1|2.911242604|[](https://articulo.mercadolibre.com.ar/MLA-678695062-cargador-universal-para-pilas-18650-14500-26650-ultrafire-_JM?variation=19019023778&quantity=1#reco_item_pos=1&reco_backend=machinalis-seller-items-pdp&reco_backend_type=low_level&reco_client=vip-seller_items-above&reco_id=7352aa27-a3d6-4223-9ae9-d8e44830d339)|
|battery holder|1|1.124260355|[](https://articulo.mercadolibre.com.ar/MLA-812596321-portapila-2-pilas-bateria-porta-pilas-doble-18650-salida-cab-_JM?quantity=1#position=1&type=item&tracking_id=08eb7c3b-f94b-4834-a1d7-e88dc6b7ab6a)|
|rechargable 18650 batteries|2|3.360946746|[](https://articulo.mercadolibre.com.ar/MLA-717530188-pila-bateria-18650-recargable-37v-6800mah-li-ion-linternas-_JM?quantity=1#position=1&type=item&tracking_id=cbb2490b-d433-4775-9784-98cee71379df)|
|LoRa module|2|15|[](https://www.ebay.com/itm/REYAX-RYLR896-Lora-module-SX1276-UART-Interface-868MHz-915MHz-Antenna-AT-command/181562403752?hash=item2a45f66ba8:g:h0QAAOSw9~5ZVKTx)|
|Hermetic case|2|8,272189349|[](https://articulo.mercadolibre.com.ar/MLA-823608945-frascos-vidrio-lunchera-hermetico-envase-recipiente-1000ml-_JM?quantity=1&variation=45946622024)|
|Electronic stuff(jumper wires, terminal boards, soldering tin, etc.)||	10||

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


### References
<div class="csl-entry">Pesce, S. F., &#38; Wunderlin, D. A. (2000). Use of water quality indices to verify the impact of Córdoba city. <i>Water Research</i>, <i>34</i>(11), 2915–2926. https://doi.org/10.1016/S0043-1354(00)00036-1</div>

















# EcoSen - Data-Loggers and sensors for environmental quality (Español abajo)
Environmental monitoring is essential due to the variety of ways in which it is threatened.
Usually recording environmental variables can be carried out by private data loggers. These devices, due to their high costs, or being of closed design, do not allow us to buy in quantity or build them.
Our proposal consists in the design and development of open hardware data loggers with LoRaWan technology for communication with devices for downloading data. The data loggers will be of two types: aquatic and terrestrial. Aquatics will measure relevant data for the determination of water quality such as turbidity, dissolved oxygen, conductivity and pH. The terrestrial, will measure bee activity variables in hive, biological indicators of environmental quality.
These data loggers are based mainly in the [Cave Pearl Proyect](https://thecavepearlproject.org/), but with adaptations to surface waters.

<img src="Images/image_1.jpg" width="100%">

### Motivation
We want to bring to society the passion for monitoring rivers and lakes. Also with the plus of learning about open electronic projects with possibility of reproduce, modify and customize data loggers. The Open technology that we bring is associated with open data repositories that will make the environmental information accessible to everyone!

### The first steps, measuring
To begin recording environmental variables is necessary to develop some abilities measuring these. To do that we are gonna start making a [Coqui conductivity sensor](https://publiclab.org/wiki/coqui) of [Public Lab](https://publiclab.org/) website.
<img src="Images/Coqui.jpg" width="100%">
With this task, we are learning to measure environmental variables with an open source hardware

### Second step, logging
To begin logging we are going to made an Arduino Uno based data logger. This data logger is based in one of the [Cave Pearl Projects] (https://thecavepearlproject.org/2015/12/22/arduino-uno-based-data-logger-with-no-soldering/). After complete the datalogger we are going to add a DHT11 temperature and relative humidity module to pin 8 of Arduino Uno. The code.ino is downloadable in the following [link](https://drive.google.com/open?id=17P1dIhY--dl7_n6sXm4gY56F4k5InGaj)or in the Codes folder.
<img src="Images/HumTeDL.jpg" width="100%">


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
|arduino pro mini|1|3.881656805|[->](https://articulo.mercadolibre.com.ar/MLA-643647762-arduino-pro-mini-33v-8mhz-robotica-atmel-atmega328-mona-_JM)|
|Arduino mega|1|9.349112426|[](https://articulo.mercadolibre.com.ar/MLA-621290099-arduino-uno-r3-atmega16u-atmega328-atmel-robotica-todomicr-_JM?quantity=1#position=9&type=item&tracking_id=982584cd-6e84-467d-a826-ffea1fc20edd)|
|temperature sensor ds18b20|1|4.130177515|[](https://articulo.mercadolibre.com.ar/MLA-818621568-sensor-digital-temperatura-ds18b20-cable-sumergible-3-metros-_JM)|
|sensor de turbidez|1|15.66863905|[](https://articulo.mercadolibre.com.ar/MLA-668633063-modulo-sensor-de-turbidez-analogico-liquid-particles-_JM)|
|pH sensor|1|29.5|[](https://www.dfrobot.com/product-1025.html)|
|conductivity sensor|1|79.9|[](https://www.dfrobot.com/product-1797.html?search=conductivity&description=true)|
|disolved oxygen sensor|1|169|[](https://www.dfrobot.com/product-1628.html)|
|real time clock|1|2.970414201|[](https://articulo.mercadolibre.com.ar/MLA-617370292-reloj-tiempo-real-rtc-ds3231-eeprom-24c32-arduino-mona-_JM)|
|18650 battery charger |1|2.911242604|[](https://articulo.mercadolibre.com.ar/MLA-678695062-cargador-universal-para-pilas-18650-14500-26650-ultrafire-_JM?variation=19019023778&quantity=1#reco_item_pos=1&reco_backend=machinalis-seller-items-pdp&reco_backend_type=low_level&reco_client=vip-seller_items-above&reco_id=7352aa27-a3d6-4223-9ae9-d8e44830d339)|
|battery holder|1|1.124260355|[](https://articulo.mercadolibre.com.ar/MLA-812596321-portapila-2-pilas-bateria-porta-pilas-doble-18650-salida-cab-_JM?quantity=1#position=1&type=item&tracking_id=08eb7c3b-f94b-4834-a1d7-e88dc6b7ab6a)|
|rechargable 18650 batteries|2|3.360946746|[](https://articulo.mercadolibre.com.ar/MLA-717530188-pila-bateria-18650-recargable-37v-6800mah-li-ion-linternas-_JM?quantity=1#position=1&type=item&tracking_id=cbb2490b-d433-4775-9784-98cee71379df)|
|LoRa module|2|15|[](https://www.ebay.com/itm/REYAX-RYLR896-Lora-module-SX1276-UART-Interface-868MHz-915MHz-Antenna-AT-command/181562403752?hash=item2a45f66ba8:g:h0QAAOSw9~5ZVKTx)|
|Hermetic case|2|8,272189349|[](https://articulo.mercadolibre.com.ar/MLA-823608945-frascos-vidrio-lunchera-hermetico-envase-recipiente-1000ml-_JM?quantity=1&variation=45946622024)|
|Electronic stuff(jumper wires, terminal boards, soldering tin, etc.)||	10||

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
