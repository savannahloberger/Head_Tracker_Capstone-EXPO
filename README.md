# Head_Tracker_Capstone-EXPO
Head Tracker for Oregon State University Engineering Expo

For helicopter pilots to make use of AR (Augmented Reality) within their displays, they need to have their head movements tracked accurately and with little latency.

# Problem Statement 

During real time flights, pilots can use tools that display augmented reality to users. However, if there is a discrepancy between the real world and what is being shown to a pilot, there can be miscommunication, loss of information, or poor decisions made by pilots based on faulty information. Because of this, our client’s goal is to create a system that is able to display an augmented reality that matches the real world with additional information to the user.

Even when using accurate sensors for reading changes in the environment, there is possibilities for errrors in the readings. By combining and averaging 6 different sensors position readings, we hope to minimize error as much as possible. 

# Project Description 

Our project is a low cost, accurate, and low-latency implementation of a head tracker that is desinged for pilots. By combining a Raspberry Pi, 6 IMU sensors, and software, we can display and track an accurate location of the pilots head. 

The software will read the data from the sensors, calculate the head position based on the data, and send the head position to the display system in real time for testing. The software will be applied to an AR system which used to improve the pilots’ safety and operation during their flight. For this project, the software is designed to read data from six IMU units and run on Linux that is installed on a Raspberry Pi. Fast, accurate, and lightweight software used for helicopter pilots display head positioning that averages IMU sensor data and corrects drift. 

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
For this software we focused on the parameters, keeping the overall system light weight and fast. The software can be described as two main components, the software library and the main function. 


The library supports the functionality required of the software:  
- Average
- Check connections
- Data 
- Display 
- Dummy (practice data)
- Logging 
- Read data 
- Run time 
- Utilities 



Requirements: 
-

- Communication with External interfaces: Rpi to IMU, RPi to Mag, Rpi to LEDs, Rpi trigger system
- Press a button to start (physical or keyboard)
- Built-In Test 
- SW functions: 
    - calculate drift at 10 Hz when system is parked
    - read sensors over time and store data in file with time change
- Sensors = 9dofs of the chip x 6 chips 
- Track relative drift and flag anomalies


# 

Team members: Eric Sisson, Jianlong Huang, and Savannah Loberger
