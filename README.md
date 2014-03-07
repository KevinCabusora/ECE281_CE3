ECE281_CE3
==========

## Moore and Mealy Advanced Elevator Controller
## C3C Kevin Cabusora
## Dr. Neebel
## ECE 281
## M6

===========================
# Moore Machine

![Moore Simulation](https://github.com/KevinCabusora/ECE281_CE3/blob/master/Moore_Testbench_Simulation.png?raw=true "Image")

[Moore VHDL](https://github.com/KevinCabusora/ECE281_CE3/blob/master/MooreElevatorController_Shell.vhd)

[Moore Testbench](https://github.com/KevinCabusora/ECE281_CE3/blob/master/Moore_testbench_Cabusora.vhd)

## Explanation
My Moore machine's output lines up with what the desired effect should be.  The elevator only goes up one floor when up_down=1 and stop=0.  Once it has gone up, it goes through 2 clock cycles.  Once the elevator has reached the 4th floor, the elevator will move down one floor at a time to the first floor when both updown and stop = 0.

==========
# Mealy Elevator Controller

![Mealy Simulation](https://github.com/KevinCabusora/ECE281_CE3/blob/master/Mealy_Testbench_Simulation.png?raw=true "Image")

[Mealy VHDL](https://github.com/KevinCabusora/ECE281_CE3/blob/master/MealyElevatorController_Shell.vhd)

[Mealy Testbench](https://github.com/KevinCabusora/ECE281_CE3/blob/master/Mealy_testbench_Cabusora.vhd)

## Explanation
The output of the testbench corresponds with that of the Moore Machine (with the only difference being the nextfloor, which is not available in the Moore) leads me to conclude that the testbench and the vhdl are set up correctly.  

==========
# Questions and Answers

Q; Is the reset synchronous or asynchronous?
A: It is synchronous.
Q: Will the Mealy Machine be different from your Moore Machine?
A: It will not be different in output, so no.
Q: What is the clock frequency? 
A: Using the formula f = 1 / T, in substituting 10ns for period we would get 100 MHz.
Q. What value would we set to simulate a 50 MHz clock?
A: Using again the f = 1 / T formula we would get 20 ns.

============
# Documentation

C3C Kyle Jonas helped point out syntax errors, mostly in the Moore and Mealy shells.
