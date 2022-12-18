# Securinets-hardware-minCTF-ISI


## Blind | 300 Point
### Difficulty : Easy 
### Description

In this link you will find a circuit [link](https://wokwi.com/projects/351112817453040216)

enjoy

The flag is in this format 

Securinets{put the flag here}

### Solution 

After opening the link we will find a circuit with simulation and a code 

![image](https://user-images.githubusercontent.com/60358423/208291604-5822d862-7173-48bc-9cfe-1d31acbc6828.png)

After simulating the circuit we find out that the led blinks with diffrent timing 
and with understunding the code we find out that it's a morse code msg 

![image](https://user-images.githubusercontent.com/60358423/208291651-4bdac990-255a-407f-8adf-fd8941afee6b.png)


```bash

#define LED 2

void setup() {
  pinMode(LED, OUTPUT);
}

void loop() {
  digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
   digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(500);
  digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
  digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(1000);
  digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
  digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(1000);
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(500);
  digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(500);
  digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(1000);
    digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
    digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
    digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
    digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(1500);

}


```



What we understund from the code is that for hight delay (500) and low delay (500) it means a . 

```bash
 digitalWrite(LED, HIGH);
  delay(500);
  digitalWrite(LED, LOW);
  delay(500);
```



And for High delay(1000)  and low delay(500) it refers to -

```bash
 digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(500);
```

and for Low delay(1000) it means that the letter ended and the next is a new letter 
for low delay(1500) it means the end of the word 

this is the morse code that we manage to find 

.-.. .. -.-. .…


L     I      C      H

Flag = Securinets{LICH}



##  Digital analyser



