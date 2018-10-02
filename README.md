# CilinderInhoud

String naam;
int diameter;
float hoogte;
const float pi = 3.14;

void setup() {
  Serial.begin(9600);
}

void loop() {
  
  Serial.println("Wat is je naam: ");
  while (Serial.available()==0) {
  
  }
  naam=Serial.readString();
  
  Serial.println("Wat is de diameter van de cilinder? ");
  while (Serial.available()==0)  {
  
  }
  diameter=Serial.parseInt();
  
  Serial.println("Wat is de hoogte van de cilinder? ");
  while (Serial.available()==0)  {
  
  }
  hoogte=Serial.parseFloat();

  Serial.print("De diameter van de cilinder is: ");
  Serial.println(diameter);
  Serial.print("De hoogte van de cilinder is: ");
  Serial.println(hoogte);
  Serial.print("De inhoud van de cilinder is: ");
  Serial.print(pi * (diameter/2) * (diameter/2) * hoogte);
  Serial.println(" cm3.");
  
 
}
