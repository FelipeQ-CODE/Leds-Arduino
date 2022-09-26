#include <stdio.h>

void setup(){
  for (int i=8; i<=11; i++)
    pinMode(i , OUTPUT);
}
void loop() {
   
    for(int i=0;i<=5; i++){
    digitalWrite(8+i, HIGH);
    delay(300);
    digitalWrite(8+i,LOW);
    delay(300);
  }
    for(int i=1;i<=4; i++){
    digitalWrite(11-i, HIGH);
    delay(300);
    digitalWrite(11-i,LOW);
    delay(300);
  }
  for (int i=1; i<=12; i++){
    digitalWrite(12+i,HIGH);
    delay(200);
    digitalWrite(12+i,LOW);
    delay(200);
}
}