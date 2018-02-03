# Line follower sensors

An array of Infrared Sensors that help the robot move along a line.

## Principle of working

The line follower sensors have the capability to detect a white line on a dark background depending on the contrast. They estimate whether the line underneath them is shifting towards the left or right as they move over them. Based on the estimation, they give respective signals to the motors to turn left or right so as to maintain a steady center with respect to the line.

These robots usually use an array of Infrared sensors in order to calculate the reflectance of the surface beneath them. The basic criteria being that the black surface will have a lesser reflectance value (black will absorb light), than the light surface which is the line.

This low reflectance value is the parameter that is used to detect the position of the line by the robot. The lower the value of reflectance will be the around the line. So in this linear array of IR sensors, if the leftmost or rightmost Infrared sensors presents the high value of reflectance, then the black line is towards the left or right of the robot respectively. The controller then compensates for this by signalling the motor to go in the opposite direction of the line. 

The Infrared Sensor consists of individual Infrared Led's and Infrared photodiodes. The Infrared light emitted by the LED strikes the surface and is reflected back to the Infrared Photodiode. The photodiode then gives an output voltage proportional to the reflectance of the surface (high value for a light surface and low for black/dark surface)

<p align="center">
	<img src="./Assets/IRsensor.jpg" />
</p>

## Circuit Design

The circuit is set up as following

<p align="center">
	<img src="./Circuit_design/Circuit.png" />
</p>

## Inventory

| Item          | Quantity      | Price (Ksh) | Total Cost | Supplier | Link |
| ------------- |---------------| ------|------------|----------|------|
| Infrared Receiver IR Transmitter Pair | 6 | 20.00 | 120.00 | Ktechnics  | https://ktechnics.com/shop/infrared-receiver-transmitter-pair/ |
| LM358N Low Power Dual Op-Amp IC | 3 | 150.00 | 450.00 | Ktechnics  | https://ktechnics.com/shop/lm358n-low-power-dual-op-amp-ic/ |
| 8 PIN DIP IC SOCKET | 3 | 10.00 | 30.00 | Ktechnics  | https://ktechnics.com/shop/8-pin-dip-ic-socket/ |
| Strip/Vero board | 4 | 50.00 | 200.00 | Ktechnics  | https://ktechnics.com/shop/stripvero-board/ |
| 4.7 Killo ohm resistor | 12 | 3.00 | 36.00 | Ktechnics  | n/a |
| 100 Ohm resistor | 6 | 3.00 | 18.00 | Ktechnics  | n/a |
| 100 Killo ohm resistor | 6 | 3.00 | 18.00 | Ktechnics  | n/a |
| Total | 872.00 Ksh |

## References

http://www.instructables.com/id/DIY-Line-Follower-Sensor-Array/

https://diyhacking.com/make-line-follower-robot/
