
# Reflections

## Describe how the paramenter of the PID controll affect the behaviour of the car

## Proportional parameter:

The proportional paramenter affect how fast the pid controll oscillates. In our example this means the reactiveness of the car on stearing, the best parameter choosen was Kp=0.1 after several trial and error. The proportional parameter was tested also isolated from the derivative and the Integral parameter choosing that a singol proportional is not enough to make the car drive around the trak. In fact we would have overshooting that never recovers.

## Derivative parameter

The derivative parameter of a PID control is used mainly to solve the overshoot problem of the proportional control. In fact using the derivative we can get a parameter of when our error is decrissing tuning up a parameter that decrease is magnitude once reacing the optimal CTE. The best parameter choosen was a Kd=0.9 that in combination with the Kp=0.1 shows up the best performance.


## Integral parameter
The Integral parameter is used for solve the problem of the Systematic Byas. Using the sum of the CTE this term can be setted for solve some error in the stearing, in fact as we act for a stear of 0.5 in reality we could have a stear of 0.4 since the mecaninc error of the attuator. This would lead to an error that the PD controller could not solve but adding the Integral controller we could solve even this error. Since we are simulating and the Systematic Byas is not affecting our simulation, the paramater choosen for the Integral was Ki=0


## Describe how the final hyperparameters were chosen.

The hyperparameters where choosen with a trial and error looking at the results in the simulator. 
