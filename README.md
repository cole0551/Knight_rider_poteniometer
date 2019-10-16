# Knight_rider_poteniometer
int potvel;
int const potPin=A1;

void setup() {
 for(int x =1; x<14;x=x+1){
  pinMode(x,OUTPUT);
  Serial.begin (9600); 
 }// end loop
 }// end setup
 
void loop() {
  // put your main code here, to run repeatedly:
  Serial.print ("the value of potvel = ");
  Serial.println (potvel);
 
  potvel=analogRead(potPin);
for(int x=0;x<14;x=x+1){
    Serial.print ("the value of potvel = ");
  Serial.println (potvel);
 
  potvel=analogRead(potPin);
digitalWrite(x,HIGH);
delay (potvel);
digitalWrite(x,LOW);

} // end for

for(int x=13;x>0;x=x-1){
    Serial.print ("the value of potvel = ");
  Serial.println (potvel);
 
  potvel=analogRead(potPin);
digitalWrite(x,HIGH);
delay (potvel);
digitalWrite(x,LOW);

} // end for

} // end void loop
