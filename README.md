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



##  Digital analyser | 300

### Difficulty : Easy 

### Description 

Someone just sent me this data but i don’t know what it is please help
all i know it's UTF-8 encoding

![Digital Analyser](https://user-images.githubusercontent.com/60358423/208293938-1838e18a-aeb2-462c-ba97-4e816f828ba5.jpeg)


## Solution

First we need to understand the message length

The time scale ends in 48 wich menas 48/8= 6 because it's a UTF-8 enconding 

which means there is 6 letters


![Digital Analyser](https://user-images.githubusercontent.com/60358423/208294859-5df26012-45bb-4b31-bde0-d8abd6e54dc9.jpg)

```bash



01110011 00110011 00111101 01001100 01101001 00110110

```

![image](https://user-images.githubusercontent.com/60358423/208294068-903d1394-9e3b-4320-b806-51bbfb7b4dff.png)


flag : Securinets{s3=Li6}



## Minetesstuuu | 500


### Difficulty : Medium  

### Description

if output = 1 when input ABCD then

flag{ABCD}

A bar is written A/

spaces and lower case are not accepted

flag = Securinets{put your flag here}
enjoy your game 


### Solution


![bin](https://user-images.githubusercontent.com/60358423/208295085-a60d189d-934c-497c-892f-58ec6239c0c8.jpg)




![image](https://user-images.githubusercontent.com/60358423/208295103-3abc9150-6ab3-4303-90f3-fd093cc0f4c8.png)




![image](https://user-images.githubusercontent.com/60358423/208295142-a692d034-3473-40f6-b9b6-c37291117468.png)




![image](https://user-images.githubusercontent.com/60358423/208295158-822d2ec1-7f7e-4d11-bb30-9b0fc71fcdd3.png)



![image](https://user-images.githubusercontent.com/60358423/208295168-3e61b06b-a693-4cc7-9cbe-7c19b025599b.png)



![image](https://user-images.githubusercontent.com/60358423/208295204-17129829-6d8a-479a-b139-048140909c7c.png)




![image](https://user-images.githubusercontent.com/60358423/208295233-0723a00f-24ea-4758-ab58-6f43e0864057.png)



![image](https://user-images.githubusercontent.com/60358423/208295258-8cf102f6-c44a-4f8f-b24c-71a5174c9fec.png)



![image](https://user-images.githubusercontent.com/60358423/208295279-2e1348f9-505c-40d9-9262-232d7a1f1010.png)



![image](https://user-images.githubusercontent.com/60358423/208295290-b3b9b508-47f1-480e-97df-69bcb4650408.png)




![image](https://user-images.githubusercontent.com/60358423/208295317-6933dcc7-6846-456f-926e-c9f8b20ede68.png)




![image](https://user-images.githubusercontent.com/60358423/208295347-e7b386a1-2d65-432f-b8eb-ca9010b502ab.png)












