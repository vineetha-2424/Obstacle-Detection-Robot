int ir = 2;
int enA = 5, in1 = 6, in2 = 7;

void setup() {
  pinMode(ir, INPUT);
  pinMode(enA, OUTPUT);
  pinMode(in1, OUTPUT);
  pinMode(in2, OUTPUT);
}

void loop() {
  if (digitalRead(ir) == LOW) {
    digitalWrite(in1, LOW);
    digitalWrite(in2, LOW);
  } else {
    digitalWrite(in1, HIGH);
    digitalWrite(in2, LOW);
  }
  analogWrite(enA, 150);
}# Obstacle-Detection-Robot
