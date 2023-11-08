# Team Members-
1. Ankita Awasthi [12140250]
2. Astha Rangare [12140350]
3. Roshni Kaushik [12141400]
4. Swati Meshram [12141670]
5. Vanshika [12141720]

# Sender code
void setup() {
  // Begin the Serial at 9600 Baud
  Serial.begin(9600);
}

void loop() {
  int a=random(0,2);
  String s=String(a);
  char b[2];
  s.toCharArray(b,2);
  for (int i=0; i<sizeof(b); i++){
      Serial.println(b[i]);
  }
  delay(1000);
}

# Receiver code
char mystr[10]; //Initialized variable to store recieved data

void setup() {
  // Begin the Serial at 9600 Baud
  Serial.begin(9600);
}

void loop() {
  Serial.readBytes(mystr,1); //Read the serial data and store in var
  Serial.print(mystr); //Print data on Serial Monitor
  delay(10);
}

![image](https://github.com/RoshniKaushik/Communication/assets/150284014/31cf23d3-01ba-406f-b9c6-2a156f7ae1d5)
![image](https://github.com/RoshniKaushik/Communication/assets/150284014/6eb3bf21-b0e9-4c8a-b841-2df2f3d002a2)
![image](https://github.com/RoshniKaushik/Communication/assets/150284014/9edc9d91-5c6e-4575-ae11-5fd7adec4af8)


