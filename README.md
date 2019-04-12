# Task-3.2
Calling a function

int ledRed = D6; 
int ledGreen = D5;
int ledBlue = D4;


void setup() {


  pinMode(ledRed, OUTPUT);
  pinMode(ledGreen, OUTPUT);
  pinMode(ledBlue, OUTPUT);
  Particle.function("led",led);

}


void loop() {



}
int led(String input)
{
    if(input == "one")
    {
        digitalWrite(ledRed,HIGH);
        
    }
    if(input == "two")
    {
        digitalWrite(ledGreen,HIGH);
    }
    if(input == "three")
    {
        digitalWrite(ledBlue,HIGH);
    }
    if(input == "1")
    {
        digitalWrite(ledRed,LOW);
        
    }
    if(input == "2")
    {
        digitalWrite(ledGreen,LOW);
    }
    if(input == "3")
    {
        digitalWrite(ledBlue,LOW);
    }
    
}
