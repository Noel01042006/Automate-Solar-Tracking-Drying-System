int LDR_front = A0;
int LDR_back = A1;

int motor1A = 8;
int motor1B = 9;

int motor2A = 10;
int motor2B = 11;

int threshold = 50;

void setup()
{
 pinMode(motor1A, OUTPUT);
 pinMode(motor1B, OUTPUT);
 pinMode(motor2A, OUTPUT);
 pinMode(motor2B, OUTPUT);
}

void loop()
{
 int front = analogRead(LDR_front);
 int back = analogRead(LDR_back);

 int difference = front - back;

 if(abs(difference) < threshold)
 {
   stopMotors();
 }
 else if(difference > threshold)
 {
   moveForward();
 }
 else
 {
   moveBackward();
 }
}

void moveForward()
{
 digitalWrite(motor1A, HIGH);
 digitalWrite(motor1B, LOW);

 digitalWrite(motor2A, HIGH);
 digitalWrite(motor2B, LOW);
}

void moveBackward()
{
 digitalWrite(motor1A, LOW);
 digitalWrite(motor1B, HIGH);

 digitalWrite(motor2A, LOW);
 digitalWrite(motor2B, HIGH);
}

void stopMotors()
{
 digitalWrite(motor1A, LOW);
 digitalWrite(motor1B, LOW);

 digitalWrite(motor2A, LOW);
 digitalWrite(motor2B, LOW);
}
