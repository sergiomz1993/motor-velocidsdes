# motor-velocidsdes
velocidades contralada por arduino
 int i;
 int digpin= 11;
 int digpin1= 7;
 int digpin2= 4;

void setup() {
}

void loop(){
for (i=0; i<=255 ; i++){
     analogWrite(digpin,i);
     digitalWrite(digpin2,HIGH);
     digitalWrite(digpin1,LOW);
     delay (10); 
}


for (i=255; i>=0 ; i--){
     analogWrite(digpin,i);
     digitalWrite(digpin2,HIGH);
     digitalWrite(digpin1,LOW);
     delay (10); 
}

for (i=0; i<=255 ; i++){
     analogWrite(digpin,i);
     digitalWrite(digpin2,LOW);
     digitalWrite(digpin1,HIGH);
     delay (10); 
}

for (i=255; i>=0 ; i--){
     analogWrite(digpin,i);
     digitalWrite(digpin2,LOW);
     digitalWrite(digpin1,HIGH);
     delay (10); 

}
}
