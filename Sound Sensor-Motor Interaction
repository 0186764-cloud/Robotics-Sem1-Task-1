const int In1 = 9;
const int In2 = 8;
const int audio = A0;

void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  pinMode(audio, INPUT);
  pinMode(In1, OUTPUT);
  pinMode(In2, OUTPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
  Serial.println(analogRead(audio));
  if ((analogRead(audio) > 10)){
    digitalWrite(In1, HIGH);
    digitalWrite(In2, LOW);
    }
  else{
    digitalWrite(In1, LOW);
    digitalWrite(In2, LOW);
  }
}
