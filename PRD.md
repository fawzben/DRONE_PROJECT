# Product requirements document

**Core Purpose:** To design, build, and program a functioning quadcopter from basic electronic components to master the intersection of CAD, electronics, and control loops    


**Out of Scope:** Autonomous waypoint navigation, long-range flight, high-speed racing, acrobatics, and camera payloads.  

1. The drone must automatically self-level when the control sticks are centered
1. The drone must be stable when control sticks are centered
  - 2 motors spin clockwise , the other 2 counter-clockwise  
1. Weight :
  Maximum Take-Off Weight of 550 grams (including the battery)  
  Target Breakdown:  
    - 3D Printed Frame & Fasteners: ≤ 160g
    - 4x Motors & Propellers: ≤ 140g
    - 4x ESCs (Electronic Speed Controllers) + Wiring: ≤ 50g
    - Battery: ≤ 150g
    - Microcontroller + IMU Sensor + RC Receiver: ≤ 50g 
1. Dimensions : 210 mm to 230 mm motor-to-motor diagonal distance  
   *allows for easier 3D-printing* 
1. Good responsiveness
  - Main loop execution frequency must be a constant 250 Hz (one calculation loop every 4 milliseconds) 
3. Able to resist air curents  
  - Thrust-to-Weight Ratio of ≥ 2:1.
4. Motor mounting arms must be rigid (or close to) to prevent twisting/bending
  - Optimised cross-section geometry
5. Battery with enough voltage
   



   
