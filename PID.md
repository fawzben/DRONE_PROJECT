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
