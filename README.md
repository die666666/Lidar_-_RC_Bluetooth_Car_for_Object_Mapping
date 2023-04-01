# Lidar_-_RC_Bluetooth_Car_for_Object_Mapping


A Lidar and RC Bluetooth car for object mapping is a cutting-edge technology that combines the power of a Lidar sensor and a Bluetooth-controlled remote control car to create a precise mapping tool. The Lidar sensor scans the environment and detects objects, while the Bluetooth car provides control and mobility. By combining these two technologies, the Lidar and RC Bluetooth car can create accurate maps of any indoor or outdoor space. This technology is useful in various industries, such as construction, mining, and urban planning, to create detailed maps and make informed decisions.

We are using YD Lidar, Motor driver L298N, Arduino Uno and HC – 06 Bluetooth module for making this project. The output is displayed on PC/Laptop and user can also control it by an Android application which will control the Buttons to guide our prototype. Coming to the design of the circuit, first is the HC-05 Bluetooth Module. The +5V and GND pins of the Bluetooth Module are connected to +5V and GND of Arduino. Since we will be only transmitting data related to the Robot’s movement from Android Phone to Bluetooth Module and do not intend to receive any data from Arduino, we will connect only the TX pin of the Bluetooth Module to RX Pin of Arduino. This RX pin of Arduino is based on Software Serial library (Pin 2 and Pin 3 are configured as RX and TX on Arduino). The RX pin of the Bluetooth is left open. 
Now, the L298N Motor Driver Module Digital I/O Pins 9 through 12 of Arduino are configured as Input pins of the Motor Driver and are connected to IN1 through IN4 of the L298N Motor Driver Module. Both the Enable Pins are connected to 5V through provided jumper. The robot chassis which I am using in this Bluetooth Controlled Robot Car project is supplied with 4 geared motors. Since L298N has slots for only two motors, I have joined the left side motors as one set and the right side motors as other set and connected both these sets to the output of  L298N Module.



Components:-
1. YDLIDAR X2 360 Degree ROS Scanner
2. Arduino Uno
3. Jumper Wires
4. HC-06 Bluetooth module
5. L298N Motor driver


Steps:-
When we supply the power to the system it will turn on the lidar and it starts rotating and our RC Bluetooth car can also get started by light indication from arduino and L298N motor driver. Whenever, user wants to start the prototype they must need to make sure that the connection are correct or not otherwise, it would be a big issue to operating it. After that give appropriate power supply to our L298N motor driver and arduino uno so that the current will flow efficiently. With arduino HC-06 bluetooth module is also connected by jumper wire. When the current flows it flows through arduino then the external power supply will also pass from Bluetooth module. And, by the combination of both will result our output.  

After connecting the lidar with your respective computer/laptop open lidarviewer which is a software that can easily convert your lidar data into an object by the help of point cloud processing.
