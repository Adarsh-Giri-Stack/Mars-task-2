Mars task-2 was similar to task one, but this time we had to do it offline with real
components and the task was given on the spot. 
the task was to use a dc motor and control it using a push button. we also had to control and adjust the speed and 
direction of spin . 
so first i thought about the components i am going to use which were as follows :
  1. potentiometer- to control speed and adjust direction
  2. power driver- since dc motor requires more than 5V , we use this to amplify the voltage
  3. arduino uno r3
  4. DC motor
  5. 9V battery

Procedure:
1)Potentiometer:
	terminal 1 to 5V arduino 
	terminal 2 to Gnd 
	wiper pin to analog pin 1
2)Power Driver:
	PWM pin to digital 6 
  Direction pin to digital 8 
	Gnd to Gnd of arduino 
3)DC motor :
	Connect to Motor pins of power driver .

4)9V Battery:
	connect to the power pins of power driver.

Logic Behind The Working :

The Potentiometer will be used as a nob to turn and adjust the speed and direction of the motor .
512 is set as the point of change. 
Raw potentiometer value ranges from 0-1023
if potentiometer value is below 512 , the motor runs in one direction 
else the motor runs in the opposite direction .
we map the value of speed from raw value 0-1023 to 0-255 .
then we print the value of speed and adjust the speed of the motor respectively.





 
	
	
