# Head_Tracker_Capstone-EXPO
Head Tracker for Oregon State University Engineering Expo

# Problem Statement 


# Project Description 


Fast, accurate, and lightweight software used for helicopter pilots display head positioning that averages IMU sensor data and corrects drift. 

Primary software tools and languages: python, C, multithreading, microcontrollers, and linux kernel environment scheduling.

# Software Desgin & Requirements
External interfaces: Rpi to IMU, RPi to Mag, Rpi to LEDs, Rpi trigger system
Press a button (physical or keyboard)
Time available (CPU or GPS?)
Built-In Test: am I talking to the cube or is it dead
SW function: calculate drift at 10 Hz when system is parked
SW function: read sensors over time, plot (?) - store data in file with timestamp accurate to XXX ascii readable (or some format)
Sensors = 9dofs of the chip x 6 chips and photodetectors if using LED system
Track relative drift and flag anomalies
Usability, performance, design constraints, software system attributes
Req and obj measurable efficiency and satisfaction, specific user test and interface
