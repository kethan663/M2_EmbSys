# Water irrigation system
## 1. About Water ieeigation system
### 1.1 Description

This project  is to create a  regulated irrigation system that will provide autonomous irrigation for plants while saving water and money. 
The major goal is to use the system to improve the soil's and hence the plant's health by using several sensors.For optimal plant growth, 
a sufficient amount of water in the soil is required. Also, because water is such an important component of life, it is necessary to limit
its use. Irrigation is the largest user of water. This necessitates the need to manage irrigation water delivery.

### 1.2 Identifying features
* It should provide the water to the plants whenever it senses the dry soil.
* It should stop the water of the motor when there is wet soil.
### 1.3 State of Art
* The key focus here is on having a motor that is intelligent enough.
* The motor should ON and OFF itself automatically.
* As the world progresses, technology must evolve to keep up.
### 1.4 5W's&1H
![5w](https://user-images.githubusercontent.com/88649955/157063478-bd4181d3-6592-4b48-a3d3-1ac3b72ad7d1.JPG)
### 1.5 SWOT Analysis
![155678758-0063bc84-e86b-4b49-9a7a-f8d0a4983a82 (1)](https://user-images.githubusercontent.com/88649955/157165148-ea08ce9b-5479-4731-ba70-149da6354302.jpg)
## 2.Requirements
### 2.1 High level requirements
| ID | High level requirements |
| ------------ | ------------- |
| HL1 | It should automatically ON the motor when the soil is dry.|
| HL2 | The motor should stop the water when there is wet soil.|
### 2.2 Low level requirements
| ID | Low level requirements |
| ------------ | ------------- |
| H1L1 | It ON the water motor accordingly to the values of soil moisture sensor.|
| H1L2 | According to the values the micro controller receives, it orders the relay to start motion.|
| H2L1 | It OFF the moto according to the timer or delay we give duing coding.|

## 3.Block Diagram and Blocks Explanation
### 3.1 Block Diagram
![ftu](https://user-images.githubusercontent.com/88649955/157182895-117e2a3a-06c6-4ab9-80ff-bd215f72222e.jpg)
### 3.2 Sensors
* Soil moisture sensor - The volumetric water content in soil is measured by soil moisture sensors.Because direct gravimetric measurement of free 
soil moisture necessitates the removal, drying, and weighing of a sample, soil moisture sensors indirectly measure the volumetric water
content by using another property of the soil as a proxy for the moisture content, such as electrical resistance, dielectric constant,
or neutron interaction. The relationship between the measured property and soil moisture must be calibrated, and it can change depending
on environmental conditions including soil type, temperature, and electric conductivity. The soil moisture affects reflected microwave 
radiation, which is employed for distant sensing in hydrology and agriculture. Farmers and gardeners can use portable probing tools.
Sensors that determine volumetric water content are commonly referred to as soil moisture sensors. Tensiometers and gypsum blocks are
examples of sensors that measure another feature of moisture in soils called water potential. These sensors are commonly referred to 
as soil water potential sensors.

### 3.3 Actuators
* DC Motor -Micro dc 3-6v micro submersible pump for fountains and gardens water circulation system for small spaces dc diy project
Submersible pump with a voltage range of 3 to 6 volts small submersible water pump micro 3v to 6vdc water pump for hobby kit homemade 
dc pump motor for a tiny submersible pump This is a low-cost, small-size submersible pump motor that runs on a 2.5- to 6-volt power 
source. It can process up to 120 litres per hour while drawing only 220 milliamps. Simply attach the tube pipe to the motor outlet, 
immerse it in water, and turn it on. Make sure the water level is higher than the motor at all times. The dry run may cause harm 
to the motor as a result of the heat, and it will also make noise.

### 3.4 Micro Controller
* The system's brain is the Micro Controller. In this project, we'll be using the Arduino UNO, which is an open-source microcontroller board made by Arduino and based on the Microchip ATmega328P microprocessor. It operates the DC motor by mapping the readings supplied by the soil moisture sensor.

## 4.Architecture
### 4.1 Behavioural Diagram
#### 4.1.1 High level flowchart behavioural diagram
![high level](https://user-images.githubusercontent.com/88649955/157183688-ccc8bac4-aecb-470a-8bfb-853d8975ff7f.JPG)
#### 4.1.2 Low level flowchart behavioural diagram
![low level](https://user-images.githubusercontent.com/88649955/157183733-e23d582c-bfb6-4cae-a573-0355d462638a.jpg)

## 5.Test Plan and Output
### 5.1 Test Plan
| Test ID | Description | Input | Expected Output | Actual Output | Passed or Not | 
| ------- | ----------- | ----- | --------------- | ------------- |-------------- |
| 1 | Soil moisture sensor | Dry soil | send 1 to micro contoller | sending 1 to micro controller |  ✅  |
| 2 | DC motor | channel relay turns ON | Rotate on receiving data from micro controller | Rotate on receiving data from micro controller |   ✅   |

### 5.2 Output
* DC motor(OFF) with wet soil
![o](https://user-images.githubusercontent.com/88649955/157179580-4c3a9fc5-836a-411b-8a40-2a4eec6b6d7f.JPG)
* DC motor(ON) on detecting Dry soil
![sef](https://user-images.githubusercontent.com/88649955/157179685-2f3643a4-3781-4bb7-8772-a677d33ae548.JPG)

## 6. Application
* Can be used at Agriculture fields, home , nusery, parks etc.
* use less amount of water.
 



