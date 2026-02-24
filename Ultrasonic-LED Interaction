// C++ code
//
const int trig = 5;
const int echo = 4;
const int led = 11;


void setup()
{
  pinMode(trig, OUTPUT);
  pinMode(echo, INPUT);  
  pinMode(led, OUTPUT);
  Serial.begin(9600);

}

void loop()
{
  long duration, cm;
  digitalWrite(trig, LOW);
  delayMicroseconds(2); 
  digitalWrite(trig, HIGH);
  delayMicroseconds(5);
  digitalWrite(trig, LOW);
  
  duration = pulseIn(echo, HIGH);
  
  cm = distanceConvert(duration);
  
  Serial.println(cm);
  if(50>cm){
    int bright = map(cm, 0, 50, 255, 0);
    analogWrite(led, bright);
    delay(1000);
  } 
  else {
    digitalWrite(led, LOW);
  }
}
long distanceConvert(long microSeconds) {
  return microSeconds / 29 / 2;
}
