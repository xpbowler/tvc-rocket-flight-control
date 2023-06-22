## About 
The software behind a thrust vector controlled (TVC) rocket - a rocket able to change its thrust direction based on attitude (orientation in 3D space). 

The program has three main steps: 
* Estimate attitude from an inertial measurement unit (IMU) and barometer by advanced sensor-fusion algorithms: Madgwick filter and Kalman filter. Uses quaternions to represent 3D orientation.
* Proportional – Integral – Derivative (PID) controller actuating servo motors in TVC mount (changing direction of thrust) 
* Live wireless flight data transmission to ground station

## Dependencies
The software is to be run on a rocket flight computer, ideally with a Teensy 4.1 microcontroller. 

Requirements: 
* System: Arduino IDE (2.1.0)
* Attitude estimation: https://github.com/xioTechnologies/Fusion
