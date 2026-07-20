-> proportional , integral , derivative

We look at the error :

*Error=Desired Angle (from your remote) − Actual Angle (from the IMU sensor)*


**P :** (present)

- Big error => big adjustement  ;  small error => small adjustment

- Problem : similarly to a spring, it overshoots, then comes back => violent tilting

**D :** (future)

- *Shock absorber* : looks at how fast the error is changing, and dampens if necessary => blocks the overshooting

**I :** (past)

- looks at overall slight neglected errors (e.g. due to wind) and corrects those


In code :



	  // 1. Calculate current error
	  float error = desired_angle - actual_angle;
	  
	  // 2. Calculate P, I, D components
	  float P = Kp * error;                       // Present error
	  float I = Ki * (previous_I + error * dt);   // Accumulated past error
	  float D = Kd * ((error - previous_error) / dt); // Speed of correction
	  
	  // 3. Total correction output to send to the motors
	  float pid_output = P + I + D;
	  
	  // Save state for the next loop (runs again in 4 milliseconds)
	  previous_error = error;


**WARNING** : 

Only works well if : 


- rigid frame (≠ flimsy)


- clean sensor data (noise cut out, with the help of a low-pass filter)


- fast loop rate (e.g. 250Hz) --> accuracy with current data, no delay




