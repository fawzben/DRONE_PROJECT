# ME-PROJECT-BUILDING-A-DRONE-FROM-SCRATCH
Summer holiday between 1st and 2nd year EPFL ME. I want to build a fully functional drone

## Entry 1 (19/07/25)

### Goal :
- Document about how drones work  
- Find subjects I will have to look into. 
- Detail a 1st PRD (cahier des charges)  

### Today's status :  

Loads of electronics, solid mechanics. Some programming, thermodynamics, fluid mechanics. 

**Key components :**

- IMU : ONBOARD sensor that gives real-time drone orientation (accelerometer, gyroscope,...)
- Batteries : 1 for each propeller, gives power for thrust
- ESCs : 1 for each propeller, tells the battery how much power to allow at each moment (speed change)
- Propellers : 2 CW , 2 CCW to cancel out forces and keep the drone still
- microcontroller : ONBOARD (probably) arduino (raspberry has OS-related delays, not optimal for high frequency commands)
- Radio receiver (controller) : transmits the user's commands to the Arduino

**Real-time process :**

1. The user does a command (ex. tilt by 10 degrees)
2. The command is radio-transmitted to the arduino
3. The IMU tells the arduino about current state (ex. titled by 8 degrees)
4. The arduino calculates the difference (e.g. here 2 degrees)
5. The arduino tells the ESCs the speed change needed to fill in that gap 

This sequence happens with a frequency of $\approx200\left\lbrack Hz\right\rbrack$

<img width="2016" height="1512" alt="IMG_6509" src="https://github.com/user-attachments/assets/d72e5b0b-19d3-4da3-b62c-cca9b946c278" />
<img width="2016" height="1512" alt="IMG_6510" src="https://github.com/user-attachments/assets/6b8217fb-f080-46a5-8d16-3c24ba5302ba" />


### Next steps :

