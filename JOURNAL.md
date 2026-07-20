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
- microcontroller : ONBOARD (probably) arduino (raspberry has OS-related delays, not optimal for high frequency commands)
- Radio controller : transmits the user's commands to the Arduino
- Radio receiver : wired to the arduino, makes the transit between the controller and the arduino

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

[[oscarliang.com]] for detailed drone info
- look at other DIY drone configuration to get an idea of what's doable and to-do
- get insight on electronic components, how to use them


## Entry 2 (20/08/25)


**What I did :**


- Learned how controller transmits to arduino

- Learned how arduino corrects errror using IMU and PID algorithm (detailed in [Tips])


- Started a "shopping list". To be completed later

- Start buying material (long shipping, and will let me start experiment coding). Bought electronics and soldering stuff

**Next steps :**


- Keep buying material (long shipping, and will let me start experiment coding)

- Set up coding environment

- Starting CADing drone frame, and do physics in parallel (e.g. total weight, to pick the right propellers)

- Do more of the physics (particularly dynamics, structure and material resistance)





