#include <SoftwareSerial.h>
SoftwareSerial mySerial(3, 2);
#define trigPin 8
#define echoPin 9
#define buzzerPin 10  // Define the buzzer pin
int redled = 13;

void setup() {
  randomSeed(analogRead(0));
  Serial.begin(9600);
  mySerial.begin(9600);
  pinMode(trigPin, OUTPUT);
  pinMode(echoPin, INPUT);
  pinMode(redled, OUTPUT);
  pinMode(buzzerPin, OUTPUT);  // Set the buzzer pin as OUTPUT
  digitalWrite(redled, LOW);
  digitalWrite(buzzerPin, LOW); // Initialize buzzer to be off
  delay(100);
}

void loop() {
  long time_duration, distance_in_cm;
  digitalWrite(trigPin, LOW);
  delayMicroseconds(2);
  digitalWrite(trigPin, HIGH);
  delayMicroseconds(10);
  digitalWrite(trigPin, LOW);
  time_duration = pulseIn(echoPin, HIGH);
  distance_in_cm = time_duration / 29 / 2;

  Serial.print(distance_in_cm);
  Serial.println(" cm");

  if (distance_in_cm >= 10) {
    digitalWrite(redled, HIGH);
    tone(buzzerPin, 1000, 50000); // Turn on the buzzer

    Serial.println("Motion detected!");
    Serial.println("calling....");

    mySerial.println("AT");
    updateSerial();

    mySerial.println("ATD+ +919663311334;");
    updateSerial();
    delay(20000);
    mySerial.println("ATH");
    updateSerial();

    delay(2000);
  } else {
    digitalWrite(redled, LOW);
    noTone(buzzerPin); // Turn off the buzzer
  }
}

void updateSerial() {
  delay(500);
  while (Serial.available()) {
    mySerial.write(Serial.read());
  }
  while (mySerial.available()) {
    Serial.write(mySerial.read());
  }
}