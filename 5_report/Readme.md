# DISTANCE MEASUREMENT SYSTEM
#  1. INTRODUCTION
## 1.1 ABSTRACT
In this project, an integrated system using an ultrasonic sensor HC-SR04 based on ATmega328P microcontroller was done. It is used to measure the distance between the system and obstracle automatically. The microcontroller is connected to ultrasonic sensor HC-SR04 which contains the piezoelectric with a particular frequency. This will generate ultrasonic waves and the waves will be reflected by the object whose distance to be measured. The time difference between the transmitted wave and reflected wave will be measured by the sensors.The accurate distance between the object and the sensors will be detected. Simulation output displayed in simulide.

## 1.2 RESEARCH
Human audible range is 20hz to 20khz. We can utilize these frequency range waves through ultrasonic sensor HC-SR04. The advantages of this sensor when interfaced with arduino which is a control and sensing system, a proper distance measurement can be made with new techniques. This distance measurement system can be widely used as range meters and as proximity detectors in industries.Ultrasonic sensor is interfaced with ATmega 328 is efficient way to measure small distances precisely. Ultrasonic detection introduces high-frequency sound waves into a test object to obtain information about the object without altering or damaging it in any way. After knowing the speed of sound the distance can be calculated.

## 1.3 FEATURES OF THE SYSTEM
1. Measures the distance automatically .

2. This system is capabile of detecting the distance of obstracle.

3. Can be used in locomotics to avoid accidents.

## 1.4 SYSTEM DESCRIPTION
In this project, we are going to interface Ultrasonic sensor HC-SR04 with ATMEGA328P and LCD Display. The ultrasonic sensor is used to measure the distance.It acts as a Sonar. It sends an ultrasonic wave of a certain frequency that comes back after hitting the object and calculates the time traveled by it. Distance Measurement Using ATMEGA 328P & HC-SR04 Ultrasonic Sensor is calculated and displayed in LCD.

## PRINCIPLE OF THE SYSTEM
An ultrasonic sensor is an electronic device that measures the distance of a target object by emitting ultrasonic sound waves and converts the reflected sound into an electrical signal. The ultrasonic sensor proposed here is a popular non-contact type level detector. It operates by generating an ultrasonic pulse and measuring the time it takes for an echo to return. The ultrasonic sensor module comprises of one transmitter and one receiver. The transmitter can deliver 40 KHz ultrasonic sound while the maximum receiver is designed to accept only 40 KHz sound waves. The receiver ultrasonic sensor that is kept next to the transmitter shall thus be able to receive reflected 40 KHz, once the module faces any obstacle in front. Thus whenever any obstacles come ahead of the ultrasonic module it calculates the time taken from sending the signals to receiving them since time and distance are related for sound waves passing through air medium at 343.2m/sec. Upon receiving the signal MC program while executed displays the data i.e. the distance measured on an LCD interfaced with the microcontroller in cms.

Ultrasonic sensors emit short, high-frequency sound pulses at regular intervals. These propagate in the air at the velocity of sound. If they strike an object, then they are reflected back as echo signals to the sensor, which itself computes the distance to the target based on the time-span between emitting the signal and receiving the echo.

We will have to convert this time into cm to calculate the distance traveled. We will use the following equation to calculate the distance.

                           S = v * t
The ultrasonic wave is basically a sound wave that travels at a speed of 340 m/s (0.034 cm/s). The ultrasonic sensor is measuring the time it takes to hit the object and then come back but we need only time that it takes to hit the object. So, we will divide it by 2.

                         S = (t * 0.034)/2                                              
## 1.5 SWOT ANALYSIS
Untitled Diagram (1)

## 1.6 4W & 1H
### WHAT
The ultrasonic sensor is used to measure the distance. It acts as a Sonar. It sends an ultrasonic wave of a certain frequency that comes back after hitting the object and calculates the time traveled by it.

### WHERE
Ultrasonic sensors are used primarily as proximity sensors. They can be found in automobile self-parking technology and anti- collision safety systems. Ultrasonic sensors are also used in robotic obstacle detection systems, as well as manufacturing technology.

### WHEN
Automatic Disrtance Measurement System can be used whereever the measurement of obstracles need to precise

### WHY
Automatic Disrtance Measurement System is the excellent method to measure the distance of the obstracles without physical needs.

### HOW
By interfacing Ultrasonic sensor with ATMega 328p with LCD the distance can be measured precisely.

# 2. REQUIREMENTS
## 2.1 HIGH LEVEL REQUIREMENTS
HLR ID	DESCRIPTION	CATEGORY	STATUS
HLR1	System shall detect the distance of the obstracle	Technical	Implemented
HLR2	System shall calculate the distance between sensor and the obstracle	Technical	Implemented
HLR3	System shall have user interface	Technical	Implemented
## 2.2 LOW LEVEL REQUIREMENTS
LLR ID	HLR ID	DESCRIPTION	CATEGORY	STATUS
LLR1	HLR1	System shall have a Ultrasonic sensor to detect the distance of the obstracle	Technical	Implemented
LLR2	HLR2	System shall have a Trigger to obtain the input	Technical	Implemented
LLR2	HLR2	System shall have a Echo to obtain the output	Technical	Implemented
LLR3	HLR3	System shall have a LCD to communicate with user to display the distance	Technical	Implemented
## 2.3 COMPONENTS REQUIRED
ATMEGA328P
Ultrasonic Sesnor HC-SR04
16*2 LCD Display
5V Power Supply
ATMEGA 328P

P.No	PIN NAME	PIN DESCRIPTION
1	Vss (Ground)	Ground pin connected to system ground
2	Vdd (+5 Volt)	Powers the LCD with +5V (4.7V – 5.3V)
3	VE (Contrast V)	Decides the contrast level of display. Grounded to get maximum contrast.
4	Register Select	Connected to Microcontroller to shift between command/data register
5	Read/Write	Used to read or write data. Normally grounded to write data to LCD
6	Enable	Connected to Microcontroller Pin and toggled between 1 and 0 for data acknowledgement
7	Data Pin 0	
8	Data Pin 1	
9	Data Pin 2	
10	Data Pin 3	
11	Data Pin 4	
12	Data Pin 5	
13	Data Pin 6	
14	Data Pin 7	
15	LED Positive	Backlight LED pin positive terminal
16	LED Negative	Backlight LED pin negative terminal

# 4. TEST PLAN AND OUTPUT
|TEST ID|	HLT ID|	DESCRIPTION	|ACTUAL OUTPUT|	PASS/FAIL|
|:------|:------|:------------|:------------|:---------|
|T_01|	H_01|	Sense the obstracles on the way of the system|	Ultrasonic sensor senses the obstracles on the way|	Pass|
|T_02|	H_02|	Trigger and echo are enabled	|The trigger and echo gives the input and output values|	Pass|
|T_03	|H_03	|Calculation of the distance between the system and obstracle	|The distance calculated is obtained	|Pass|
|T_04	|H_04	|Display of the distance between the system and obstracle	|The distance measured is displayed in LCD	|Pass|
|T_05	|H_05	|Indication when the obstracle is not found	|The details captured is displayed in LCD	|Pass|


