//PHOTORESISTANCE WITH ARDUINO

#define photoresistance_pin A5
float photoValue, photoAnalogValue = 0;

void setup() {
  pinMode(photoresistance_pin, INPUT_PULLUP);
  Serial.begin(9600);
}

void photoReader(){
  photoAnalogValue = analogRead(photoresistance_pin);
  photoValue = map(photoAnalogValue, 0, 1023, 0, 5);
}

void loop() {
  photoReader();
  Serial.println(photoAnalogValue);
  delay(2000);
}
