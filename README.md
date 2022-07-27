#include <Servo.h>

int pos = 0;

Servo servo_9;

void setup()
{
  servo_9.attach(9, 500, 2500);
}

void loop()
{
  // sweep the servo from 0 to 360 degrees in steps
  // of 1 degrees
  for (pos = 0; pos <= 360; pos += 1) {
    // tell servo to go to position in variable 'pos'
    servo_9.write(pos);
    // wait 15 ms for servo to reach the position
    delay(1); // Wait for 1 millisecond(s)
  }
  for (pos = 360; pos >= 0; pos -= 1) {
    // tell servo to go to position in variable 'pos'
    servo_9.write(pos);
    // wait 15 ms for servo to reach the position
    delay(15); // Wait for 15 millisecond(s)
  }
(س

(س
// C++ code
//
void setup()
{
  pinMode(11, OUTPUT);
}

void loop()
{
  analogWrite(11,255);
}
