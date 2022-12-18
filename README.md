# Securinets-hardware-miniCTF-ISI


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

After simulating the circuit we find out that the led blinks with different timing 
and with understanding the code we find out that it's a morse code msg 

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



What we understand from the code is that for high delay (500) and low delay (500) it means a . 

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

Flag / Securinets{LICH}



##  Digital analyser | 300

### Difficulty : Easy 

### Description 

Someone just sent me this data but i don’t know what it is please help
all i know it's UTF-8 encoding

![Digital Analyser](https://user-images.githubusercontent.com/60358423/208293938-1838e18a-aeb2-462c-ba97-4e816f828ba5.jpeg)


## Solution

First we need to understand the message length

The time scale ends in 48 wHich menas 48/8= 6 because it's a UTF-8 encoding 

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


First we opened minetest game in bin folder

![bin](https://user-images.githubusercontent.com/60358423/208295085-a60d189d-934c-497c-892f-58ec6239c0c8.jpg)




![image](https://user-images.githubusercontent.com/60358423/208295103-3abc9150-6ab3-4303-90f3-fd093cc0f4c8.png)



In the world we find a circuit and some letters and a logic gates 

![image](https://user-images.githubusercontent.com/60358423/208295142-a692d034-3473-40f6-b9b6-c37291117468.png)




![image](https://user-images.githubusercontent.com/60358423/208295158-822d2ec1-7f7e-4d11-bb30-9b0fc71fcdd3.png)

we find also a switch


![image](https://user-images.githubusercontent.com/60358423/208295168-3e61b06b-a693-4cc7-9cbe-7c19b025599b.png)


now this is the full circuit from the top 

![image](https://user-images.githubusercontent.com/60358423/208295204-17129829-6d8a-479a-b139-048140909c7c.png)


which also looks like this i've used the LOGISIM Software

![image](https://user-images.githubusercontent.com/60358423/208295943-90ec2877-2a09-4075-b72a-fea307a68f5c.png)


so the flag is the output equation that makes the blue led = 1 which is connected using the logic gates AND , OR and NOT 

![image](https://user-images.githubusercontent.com/60358423/208295233-0723a00f-24ea-4758-ab58-6f43e0864057.png)



![image](https://user-images.githubusercontent.com/60358423/208295258-8cf102f6-c44a-4f8f-b24c-71a5174c9fec.png)


after switchin on and off the switch we can see the blue led is on 

![image](https://user-images.githubusercontent.com/60358423/208295279-2e1348f9-505c-40d9-9262-232d7a1f1010.png)



![image](https://user-images.githubusercontent.com/60358423/208295290-b3b9b508-47f1-480e-97df-69bcb4650408.png)




![image](https://user-images.githubusercontent.com/60358423/208295317-6933dcc7-6846-456f-926e-c9f8b20ede68.png)


Now we need to read the letters from the other side to get the right order 
so it's CADB 

![image](https://user-images.githubusercontent.com/60358423/208295347-e7b386a1-2d65-432f-b8eb-ca9010b502ab.png)




now we found 2 solution for the OUTPUT =1 

CADB/ OR CADB/

So the output = CADB/+CAD/B
Or output = CAD/B+CADB/

flag : Securinets{CAD/B+CADB/}

or

flag : Securinets{CADB/+CAD/B}




## Escape Room | 800 points


### Description :

can you manage to find all the hidden flags ?

enjoy the game

Securinets{put your flags here}

no spaces allowed



### Solution 

After we get into the world let's try exploiting the game 

![image](https://user-images.githubusercontent.com/60358423/208297997-04fc6b4e-d5ae-4dd6-b5af-db5078095ac4.png)

We found an LCd with "guess the password" and password :BS1XFW7sML93pT9ycQxCqM

![image](https://user-images.githubusercontent.com/60358423/208298034-1dc6b643-9c17-43f1-9499-45bf007e4038.png)

BS1XFW7sML93pT9ycQxCqM is base58

![image](https://user-images.githubusercontent.com/60358423/208298199-79edca67-01dd-4cc8-9067-3211f2f7661e.png)

okey so the password is : TyManaarfch aleh

![image](https://user-images.githubusercontent.com/60358423/208298252-2a875c02-9a9a-490c-95a0-b5ff75440eaa.png)
If we look close we will see "write the password here " so we will enter the password 

![image](https://user-images.githubusercontent.com/60358423/208298368-5db24d2b-7701-4bbf-b298-681596da6f2c.png)


and here we got a flag "hOpeAmALtouJ4w"

![image](https://user-images.githubusercontent.com/60358423/208298403-81652083-c002-41b4-b9aa-2cf86437580f.png)

now this can be salved in an easier way 
so if we look close we willl find out that the LCD are controlled using a microcontroller so if we follow the circuit cable we will see that there is a microcontroller behind the wall 



![lcd](https://user-images.githubusercontent.com/60358423/208298994-40532b1b-8d96-4335-bd9c-767a69d9d34c.jpg)
![image](https://user-images.githubusercontent.com/60358423/208299019-7c1b656e-17fe-44f6-982d-399776496de3.png)

and here we find a microcontroller 

![image](https://user-images.githubusercontent.com/60358423/208299049-fbde9531-eb3b-4c31-ad36-e9ba3e7104dd.png)

![image](https://user-images.githubusercontent.com/60358423/208299068-e9ce1427-75ac-43da-b7e2-48ea8b29128c.png)


now let's look for the next flag 
we find a computer 

![image](https://user-images.githubusercontent.com/60358423/208299094-4657a674-72df-42b8-a5ac-2794ce72601e.png)
![image](https://user-images.githubusercontent.com/60358423/208299103-22429814-7b7f-41cf-b85d-d6f8c750e848.png)

there is a notepad ut it's empty so let's load a project 
![image](https://user-images.githubusercontent.com/60358423/208299117-eaff267d-cca0-4fd2-9a50-08328e679e0a.png)

we found this 
![image](https://user-images.githubusercontent.com/60358423/208299154-156e5e68-f2c3-47b7-b29c-839b3329e6d1.png)

![image](https://user-images.githubusercontent.com/60358423/208299173-c7959a87-46f7-4284-92aa-5839c907849f.png)

it's encoded message so let's try to decode it 
 the base64 returned a binary
![image](https://user-images.githubusercontent.com/60358423/208299252-a19f09c3-1778-400d-9360-76f97e8ac228.png)


so the output is : 

welcome to game 1 
you got the first part of the flag M1n3T3ssT3

here is our first flag : M1n3T3ssT3 
now after we find our second flag let's keep looking 

![image](https://user-images.githubusercontent.com/60358423/208299381-c40231a1-7ccc-46c1-a8cb-8ac9b9375c9c.png)

![image](https://user-images.githubusercontent.com/60358423/208299400-c454fdeb-b852-4fa4-baef-e5161c0199c2.png)

![image](https://user-images.githubusercontent.com/60358423/208299374-cb9a62b4-c88b-4e5b-a647-ebbc8d8a131b.png)

now in the chests we found 4 USB with flag name so let's get back into the computer 


let's connect the USB to the computer and see what we can find 

![image](https://user-images.githubusercontent.com/60358423/208299512-c57b6a87-1dd0-4308-8016-b1346913b92d.png)

this is the available command  
![image](https://user-images.githubusercontent.com/60358423/208299584-2cacd572-e975-4008-934d-c48080086674.png)

but it keep showing that the USB are empty 

![image](https://user-images.githubusercontent.com/60358423/208299693-ee92cf7c-3689-4d05-a6da-8faaa688efe8.png)


![image](https://user-images.githubusercontent.com/60358423/208299714-302c580c-e2c8-4344-a14f-acf3ae1c90d3.png)


![image](https://user-images.githubusercontent.com/60358423/208299733-0050ec29-a3c8-4599-b597-2e6a1f46108b.png)

So the file Flag3 only show us flag 3 so we understand that we are looki,g for our last flag3 
![image](https://user-images.githubusercontent.com/60358423/208299751-c62b1679-4b9e-47bd-abaa-2d675cc10c7c.png)

the next file flag shows us this
which is a morse code 

![image](https://user-images.githubusercontent.com/60358423/208299773-863f0553-fa81-4d84-af86-a6f7ad434013.png)

so it wil look like this :

-... .---- .-. -.-. .... .---- .--- .--- .--

which means : 

b1rch1jjw



so the flag : Securinets{M1n3T3ssT3hOpeAmALtouJ4wb1rch1jjw}











