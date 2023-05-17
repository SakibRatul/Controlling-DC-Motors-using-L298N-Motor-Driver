Now, as we have seen how to control the dc motor through the motor driver, let 
us do a demonstration by showing you how to control two DC motors using this 
driver.
Required Equipment
1. Arduino UNO
2. L289N Motor driver Module
3. External 3-12 V power supply
4. 2 DC Motors
5. Connecting Wires
IN1 IN2 Motor Action
1 (HIGH) 1 OFF
1 0 (LOW) Backward
0 1 Forward
0 0 OFF
We are using TT DC gear motors for this project. They require an operating 
voltage of 3-12V DC where the recommended operating voltage is 3-6V DC. 
Thus we will use 4xAA batteries (4×1.5V = 6V) to supply power for the DC 
motors. Each of the motor’s terminal is connected at OUT1, OUT2 for motor A 
and OUT3, OUT4 for motor B respectively.
We are keeping the 5V Enable jumper in its place as it will power up the L298N 
motor driver. Then, we have connected the input pins IN1, IN2, IN3 and IN4 with 
digital pins of the Arduino UNO. We have used GPIO9, GPIO8, GPIO7 and 
GPIO6 respectively to connect with each of the input pins of the motor driver. 
The enable pins ENA and ENB are connected with the digital PWM pins of the 
Arduino UNO board. We have used GPIO10 to connect with ENA and GPIO5
with ENB.
