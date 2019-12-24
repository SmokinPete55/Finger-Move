// Finger-Move
// Initial Test for finger movement
#include <Servo.h> 
Servo myservo; // create servo object to control a servo int angle = 0;	// variable to store the servo position 
void setup() { 
264 
|	Chapter 8: Physical Output 
} 
myservo.attach(9); // attaches the servo on pin 10 to the servo object void loop() { 
} 
for(angle = 0; angle < 180; angle += 1) // goes from 0 degrees to 180 degrees 
{
myservo.write(angle); delay(20);
// in steps of 1 degree // tell servo to go to position in variable 'angle' // waits 20ms between servo commands 
}
for(angle = 180; angle >= 1; angle -= 1) // goes from 180 degrees to 0 degrees { 
}
myservo.write(pos); delay(20);
// tell servo to go to position in variable 'pos' // waits 20ms between servo commands
