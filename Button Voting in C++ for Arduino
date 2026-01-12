int buttonPin13 = 13; //1st button
int buttonPin12 = 12; //2nd button
int buttonPin11 = 11; //3rd button

int ledPin = 2; //Green LED Pin


void setup() {
  //Defines the role of each pin
  pinMode(buttonPin13, INPUT_PULLUP);
  pinMode(buttonPin12, INPUT_PULLUP);
  pinMode(buttonPin11, INPUT_PULLUP);

  pinMode(ledPin, OUTPUT);
}

void loop() {
  // Read the Pins
    int a = digitalRead(13); // The NOT Gate was included due to INTPUT_PULLUP making it so that a Press = 0, and a Release = 1
    int b = digitalRead(12); // It reads it automatically as one to prevent random static and electrical noise, so a NOT gate fixes it
    int c = digitalRead(11);

  // Logical Function
    bool buttonVote = (a + b + c) <= 1;
  
  // Turning on LED if vote passes
  digitalWrite(ledPin, buttonVote);

  delay(100); //Increased for less "jumpy-ness"
}
//January 11th, 2026
