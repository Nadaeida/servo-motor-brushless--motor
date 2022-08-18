# servo-motor-

The steps of servo motor is:
The supply of the motor must be connected ( 5V and ground GND) First, Create a funtion to power servo motors after that declare the angle of motors rotation then, give a signal to the motors and this signal is from pin 13 from the arduino uno r3 then do a for loop to control of motor rotation. if the angle of rotation is from 0 to smaller than or equal 180, the motors rotates in counterclockwise direction for 15 millisecond. if the angle of rotation is equal to 180 to greater than or equal to 0, the motors rotates in clockwise for 15 millisecond.

the code :
// C++ code

//
#include<Servo.h>
Servo servoequiv;
int pos = 0;
void setup()
{
  servoequiv.attach(13);  //because I have connected signal pin with 13
  
}

void loop()
{
  // rotate from 0 to 180 degree
  for(pos=0;pos<=180;pos++)
  {
    servoequiv.write(pos);
    delay(15);
  }
  for(pos=180;pos>=0;pos--);
  {
    servoequiv.write(pos);
    delay(15);
  }
}
About brushless motor :
1- connecting the wires like the circuit:
![brushless](https://user-images.githubusercontent.c
https://user-images.githubusercontent.com/108246979/185382390-4882bbc4-469b-43dc-8571-4c5e0051599e.mp4

om/108246979/185381363-1ddd28be-ea80-4ed2-804e-8e4971530bdc.png)
![brushless2](https://user-images.githubusercontent.com/108246979/185381706-aa1d38ec-d8bc-4d7b-99a6-183e44c2d0c4.png)

2-step2:Run the brushless motor:
https://user-images.githubusercontent.com/108246979/185382480-92838a7a-9625-4ee3-94b0-01157e739734.mp4


