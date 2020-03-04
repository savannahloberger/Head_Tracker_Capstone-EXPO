# Head_Tracker_Capstone-EXPO
Head Tracker for Oregon State University Engineering Expo


# Problem Statement 

For helicopter pilots to make use of AR (Augmented Reality) within their displays, they need to have their head movements tracked accurately and with little latency.

# Project Description 

Our project is a low cost, accurate, and low-latency implementation of a head tracker that is desinged for pilots. By combining a Raspberry Pi, 6 IMU sensors, and software, we can display and track an accurate location of the pilots head. 

Fast, accurate, and lightweight software used for helicopter pilots display head positioning that averages IMU sensor data and corrects drift. 

Primary software tools and languages: python, C, multithreading, microcontrollers, and linux kernel environment scheduling. 

Benefits of new design: 
* Light weight
* Accurate
* Low cost 

# System Design & Requirements 

Design: 
- 
There are 4 steps that the data flows through: 
1. The sensors collect data readings 
2. The sensor data is interpreted and averaged on a microcontroller (in our case a Raspberry Pi) 
3. The data is then sent to a server and the AR display software modifies the image based on the input
4. The pilot sees the updated display on their glasses 

Requirements: 
- 
Main functions that will be included in the software are: 
- Calculate data from other systems / sensors 
- Functionally read sensors over time
- Correct drift in the inertial sensors
- Calculate and correct drift at 10Hz
- Display and send real time position
- Store data in file(s) with timestamps
- Output data through system socket interface



# Software Design & Requirements

Design: 
- 



Requirements: 
-
- External interfaces: Rpi to IMU, RPi to Mag, Rpi to LEDs, Rpi trigger system
- Press a button (physical or keyboard)
- Time available (CPU or GPS?)
- Built-In Test: am I talking to the cube or is it dead
- SW functions: 
    - calculate drift at 10 Hz when system is parked
    - read sensors over time, plot (?) - store data in file with timestamp accurate to XXX ascii readable (or some format)
- Sensors = 9dofs of the chip x 6 chips and photodetectors if using LED system
- Track relative drift and flag anomalies



