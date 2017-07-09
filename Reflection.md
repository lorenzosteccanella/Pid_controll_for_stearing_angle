
# Reflections

## Describe how the parameters of the PID control affect the behaviour of the car 

## Proportional parameter:

The proportional parameters affect how fast the PID control oscillates. In our example, this means the restiveness of the car on starting, the best parameter chosen was Kp=0. 1 after several trial and error. The proportional parameter was tested also isolated from the derivative and the Integral parameter choosing that a single proportional is not enough to make the car drive around the track. In fact, we would have overshot that never recovers.

## Derivative parameter

The derivative parameter of a PID control is used mainly to solve the overshoot problem of the proportional control. In fact, using the derivative we can get a parameter of when our error is decreasing tuning up a parameter that decrease is magnitude once reaching the optimal CTE. The best parameter chosen was a Kd=0. 9 that in combination with the Kp=0. 1 shows up the best performance.


## Integral parameter

The Integral parameter is used for solving the problem of the Systematic Byas. Using the sum of the CTE this term can be set for solving some error in the steering, in fact, as we act for a steer of 0.5 in reality we could have a steer of 0.4 since the mechanic error of the actuator. This would lead to an error that the PD controller could not solve, but adding the Integral controller we could solve even this error. Since we are simulating and the Systematic Byas is not affecting our simulation, the parameter chosen for the Integral was Ki=0

## Describe how the final hyperparameters were chosen.

The hyperparameters were chosen with a trial and error looking at the results in the simulator. 
