# Arduino

https://www.tinkercad.com/things/cb9pj1o9aDG-sensor-de-gas

// C++ code
//
void setup()
{
  pinMode(A0, INPUT);
  pinMode(7, OUTPUT);
  pinMode(6, OUTPUT);
}

void loop()
{
  if (analogRead(A0) > 500) {
    digitalWrite(7, HIGH);
    digitalWrite(6, HIGH);
    delay(3000); // Wait for 5000 millisecond(s)
  }
  digitalWrite(7, LOW);
  digitalWrite(6, LOW);
  delay(2000); // Wait for 3000 millisecond(s)
}
