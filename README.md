# Mechatronics
Mechatronics homework documentation

# week 2
![week2pic1](https://github.com/stellaczh/Mechatronics/blob/master/week2/week2pic1.png)
![week2pic2](https://github.com/stellaczh/Mechatronics/blob/master/week2/week2pic2.GIF)
![week2pic3](https://github.com/stellaczh/Mechatronics/blob/master/week2/week2pic3.GIF)

# week3
![week3pic1](https://github.com/stellaczh/Mechatronics/blob/master/week3/week3pic1.png)
![week3pic2](https://github.com/stellaczh/Mechatronics/blob/master/week3/week3pic2.png)

# week 4
![week4pic1](https://github.com/stellaczh/Mechatronics/blob/master/week4/week4pic1.png)
![week4pic2](https://github.com/stellaczh/Mechatronics/blob/master/week4/week4pic2.png)
![week4pic3](https://github.com/stellaczh/Mechatronics/blob/master/week4/week4pic3.png)
![week4pic4](https://github.com/stellaczh/Mechatronics/blob/master/week4/week4pic4.GIF)

# week 5
![week5pic1](https://github.com/stellaczh/Mechatronics/blob/master/week5/week5pic1.png)
![week5pic2](https://github.com/stellaczh/Mechatronics/blob/master/week5/week5pic2.GIF)
![week5pic3](https://github.com/stellaczh/Mechatronics/blob/master/week5/week5pic3.png)

code:
void setup() {
  // put your setup code here, to run once:
pinMode(13, OUTPUT);
pinMode(12, OUTPUT);
pinMode(11, OUTPUT);
pinMode(10, OUTPUT);
pinMode(7, OUTPUT);
pinMode(6, OUTPUT);
pinMode(5, OUTPUT);
pinMode(4, OUTPUT);
}

void loop() {
delay(2*1000);

//morse code S
digitalWrite(13, HIGH);
delay(0.5*1000);
digitalWrite(11, HIGH);
delay(0.5*1000);
digitalWrite(7, HIGH);
delay(0.5*1000);
digitalWrite(13, LOW);
digitalWrite(11, LOW);
digitalWrite(7, LOW);
delay(1*1000);

//morse code T
digitalWrite(13, HIGH);
delay(0.25*1000);
digitalWrite(12, HIGH);
delay(0.75*1000);
digitalWrite(13, LOW);
digitalWrite(12, LOW);
delay(1*1000);

//morse code E
digitalWrite(13, HIGH);
delay(0.5*1000);
digitalWrite(13, LOW);
delay(1.5*1000);

//morse code L
digitalWrite(13, HIGH);
delay(0.5*1000);
digitalWrite(11, HIGH);
delay(0.25*1000);
digitalWrite(10, HIGH);
delay(0.75*1000);
digitalWrite(6, HIGH);
delay(0.5*1000);
digitalWrite(4, HIGH);
delay(0.5*1000);
digitalWrite(13, LOW);
digitalWrite(11, LOW);
digitalWrite(10, LOW);
digitalWrite(6, LOW);
digitalWrite(4, LOW);
delay(1*1000);

//morse code L
digitalWrite(13, HIGH);
delay(0.5*1000);
digitalWrite(11, HIGH);
delay(0.25*1000);
digitalWrite(10, HIGH);
delay(0.75*1000);
digitalWrite(6, HIGH);
delay(0.5*1000);
digitalWrite(4, HIGH);
delay(0.5*1000);
digitalWrite(13, LOW);
digitalWrite(11, LOW);
digitalWrite(10, LOW);
digitalWrite(6, LOW);
digitalWrite(4, LOW);
delay(1*1000);

//morse code A
digitalWrite(13, HIGH);
delay(0.5*1000);
digitalWrite(11, HIGH);
delay(0.25*1000);
digitalWrite(10, HIGH);
delay(0.75*1000);
digitalWrite(13, LOW);
digitalWrite(11, LOW);
digitalWrite(10, LOW);
delay(1.5*1000);

//refresh
digitalWrite(13, HIGH);
delay(0.1*1000);
digitalWrite(12, HIGH);
delay(0.1*1000);
digitalWrite(11, HIGH);
delay(0.1*1000);
digitalWrite(10, HIGH);
delay(0.1*1000);
digitalWrite(7, HIGH);
delay(0.1*1000);
digitalWrite(6, HIGH);
delay(0.1*1000);
digitalWrite(5, HIGH);
delay(0.1*1000);
digitalWrite(4, HIGH);
delay(0.1*1000);
digitalWrite(13, LOW);
digitalWrite(12, LOW);
digitalWrite(11, LOW);
digitalWrite(10, LOW);
digitalWrite(7, LOW);
digitalWrite(6, LOW);
digitalWrite(5, LOW);
digitalWrite(4, LOW);
}


