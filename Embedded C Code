#include <Servo.h>

const int alcoholSensor = A0;    // MQ-3 connected to A0
const int buzzer = 8;
const int threshold = 400;       // Adjust based on testing
Servo brakeServo;

void setup() {
  Serial.begin(9600);
  pinMode(buzzer, OUTPUT);
  brakeServo.attach(9);  // Servo on pin 9
  brakeServo.write(0);   // Brake released
  delay(1000);
}

void loop() {
  int alcoholLevel = analogRead(alcoholSensor);
  Serial.print("Alcohol Level: ");
  Serial.println(alcoholLevel);

  if (alcoholLevel > threshold) {
    digitalWrite(buzzer, HIGH);
    brakeServo.write(90); // Engage brake
    Serial.println("ALCOHOL DETECTED! Vehicle stopped.");
    // Place GSM or WiFi alert code here
  } else {
    digitalWrite(buzzer, LOW);
    brakeServo.write(0); // Release brake
    Serial.println("Driver is sober. Vehicle can move.");
  }

  delay(1000);
}
