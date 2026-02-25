const int pot = A0;

Servo myservo;

void setup() {
  myservo.attach(9);
  Serial.begin(9600);
  pinMode(pot, INPUT);
}

void loop(){
  int input = analogRead(pot);
  input = map(input, 0, 0123, 0, 360);
  myservo.write(0);
  Serial.println(myservo.read());
  delay(500);
  myservo.write(input);
  Serial.println(myservo.read());
  delay(500);

}
