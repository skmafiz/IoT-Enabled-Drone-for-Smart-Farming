## IoT-Enabled-Drone-for-Smart-Farming
![IoT-Enabled-Drone-for-Smart-Farming](https://github.com/skmafiz/IoT-Enabled-Drone-for-Smart-Farming/blob/main/Drone.jpg)

## Abstract
India is one of the most significant income earners in the agriculture sector. As per the latest research, the productivity rate of crops in India in the field of agriculture is very high which is a considerable number of primary sources of livelihood. It requires pesticides, crop diseases, fertilizers, and other elements for agriculture, but managing such things over wide areas of fertile lands becomes very difficult. If there are fewer farmers on the arable land than is required, it won&#39;t be easy to maintain that land. To avoid these severe problems, we are developing a project: &quot;IoT-Based Drone for Smart Farming.&quot; This project involves the development of smart farming with the application of advanced IoT technologies attached to drone capabilities. Our newest concept is using IoT-enabled sensors, analytical real-time data collection of important farming parameters, advanced communication protocols like MQTT (Message Queue Telemetry Transport) enabling seamless connectivity between the drone and cloud-based platforms for remote monitoring and mapping of cropping areas, health report of crops, improving irrigation systems in relation to soil moisture, temperature, and humidity. The various precision features of the drone with the automated irrigation, precision spraying, and pest detection. It focuses on sustainability, scalability, efficiency, and resource optimization for sustainable farming techniques.

## Requirements
•	Brushless DC motors with bullet connectors\
•	ESC\
•	Hexa S550 frame\
•	Lipo Battery\
•	Lipo balance charger\
•	Power module\
•	PDB board with XT60/T connector\
•	Flight controller\
•	PPM encoder/decoder\
•	Transmitter and receiver\
•	Telemetry\
•	GPS\
•	Propellers\
•	Flight controller status indicator\
•	Buzzer\
•	Shock absorber\
•	Vero board\
•	Jumper wires\
•	Pump motor\
•	Pipe (1 m)\
•	5way connector\
•	Nozzles\
•	Water tank (500 ml)\
•	Servo motor\
•	I2C transfer board\
•	Mission Planner (Software)

##  Block Diagram
![Block Diagram](https://github.com/skmafiz/IoT-Enabled-Drone-for-Smart-Farming/blob/main/Block%20Diagram.jpg)
The block diagram illustrates an IoT-based smart farming drone system, highlighting power distribution, flight control, six brushless motors with six ESCs, GPS navigation, a pesticide spraying mechanism, radio communication. It enables autonomous flight, precision spraying for improved farming efficiency.

## Modular Connections
![Modular Connections](https://github.com/skmafiz/IoT-Enabled-Drone-for-Smart-Farming/blob/main/Modular%20Connections.jpg)
According to the below connection diagram, each motor is connected to the ESC (electronic speed controller). Each ESC signal lead is connected in the main out of the Radiolink CrossFlight V1.0 flight controller and the power leads are connected to the PDB (power distribution board). The battery is connected to the input power lead of the power module and the signal lead of the power module is connected to the flight controller, whereas the output power lead of the power module is connected to the PDB. The receiver is connected to the PPM encoder and the output of the encoder is connected to the “RC in” of Radiolink CrossFlight flight controller. The limit switch, buzzer, and GPS (global positioning system) are also connected to Pixhawk flight controller. The servo is connected to the main out of the Radiolink CrossFlight flight controller. The Pump motor circuit is closed through the servo motor.

## Implementation
In Block Diagram, connect the input power leads of ESCs (Electronic Speed Controllers) to the power distribution board and connect the output leads to the motor. Connect the yellow lead to the motor yellow lead and connect the red and black lead to the motor red and black lead vice versa to change the direction of the motor. Then connect the flight controller with ESCs (Electronic Speed Controllers) and connect a power module with the power distribution board, flight controller and battery. Then connect the GPS (Global Positioning System), telemetry, receiver, buzzer, and switch to the flight controller. Next, perform the programming and calibrations in mission planner software. The flight controller uses PPM (Pulse Position Modulation), and the transmitter uses PWM (Pulse Width Modulation). So, we need to use a PPM encoder module in the receiver where the PWM (Pulse Width Modulation) signal converts into a PPM (Pulse Position Modulation) signal.

Firstly, connect the battery to the PDB (Power Distribution Board) to energize the drone. Then turn on the transmitter to bind to the drone with it. After this, when we push the throttle up, the receiver gives the signal to the FC (flight controller). After this the flight controller gives a signal to the motor through the ESC (Electronic Speed Controller), and the motor creates thrust to lift the drone upwards straight. Similarly, when we need to move the drone forward, backward, left, right, or rotate according to its own axis, we need to click or push different buttons on the transmitter and the signal goes to the receiver, which sends the data to the flight controller. The flight controller sends different signals to the motor through the ESC (Electronic Speed Controller), and the motors rotate differently according to the transmitter order.
 
There are some auxiliary channels to control different sensors or motors. In my case, a servo motor is used to turn on the pump motor to spray. The GND pin of the pump motor is connected to the PDB (Power Distribution Board), and the +ve pin is connected through the servo arm to the PDB (Power Distribution Board). There is a spraying tank, which is connected to the pump motor through a pipe, and the spraying nozzle is connected to the output of the pump motor. When the transmitter gives a signal to the servo motor to arm down, then the circuit path is closed, and it starts spraying.

## Conclusion
Drones have formerly extensively altered agricultural assiduity and will continue to grow in the coming times. While drone use is getting more useful to small growers, there is still a way to go before they come part of every planter’s outfit canon, particularly in developing nations. Regulations around drone use need to be made and revised in numerous countries, and further exploration needs to be done on their effectiveness at certain tasks, such as fungicide operation and spraying. There are numerous ways drones can be useful to growers, but it is important to understand their limitations and functions before investing in a precious outfit. Drone Deploy, an agrarian drone supplier and programming company, suggests starting small and incorporating drone data into your association sluggishly for the stylish results.

• [Testing the precision spraying ](https://drive.google.com/file/d/1CK0vqruPO8METW7FCmbB0QqVdASAoJiB/view?usp=sharing)

• [Autonomous mode ](https://drive.google.com/file/d/167ilqC1p99xjkiIHNX3LDLYjBMY1oPVP/view?usp=sharing)

• [Loiter (position hold mode), Altitude hold mode and RTL (return to launch) features testing](https://drive.google.com/file/d/1rQN6e9pxtuWrldaFWYM3D_GxEpXNIOds/view?usp=sharing)


