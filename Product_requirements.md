# Product requirements document

**Core Purpose:** To design, build, and program a functioning quadcopter from basic electronic components to master the intersection of CAD, electronics, and control loops    

**Out of Scope:** Autonomous waypoint navigation, long-range flight, high-speed racing, acrobatics, camera payloads

1. The drone must automatically self-level when the control sticks are centered
2. The drone must be stable when control sticks are centered
  - 2 motors spin clockwise , the other 2 counter-clockwise  
3. Weight :
  Maximum Take-Off Weight of 550 grams (including the battery)  
  Target Breakdown:  
    - 3D Printed Frame & Fasteners: ≤ 160g
    - 4x Motors & Propellers: ≤ 140g
    - 4x ESCs (Electronic Speed Controllers) + Wiring: ≤ 50g
    - Battery: ≤ 150g
    - Microcontroller + IMU Sensor + RC Receiver: ≤ 50g 
4. Dimensions : 
	210 mm to 230 mm motor-to-motor diagonal distance  
   *allows for easier 3D-printing* 
5. Good responsiveness
  - Main loop execution frequency must be a constant 250 Hz (one calculation loop every 4 milliseconds) or at least 200 Hz
6. Able to resist air currents  
  - Thrust-to-Weight Ratio of ≥ 2:1.
7. Motor mounting arms must be rigid (or close to) to prevent twisting/bending
  - Optimised cross-section geometry
8. Battery with enough voltage (develop later)
   



   
