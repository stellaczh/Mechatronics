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

cod;
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

# week 6
![week6pic1](https://github.com/stellaczh/Mechatronics/blob/master/week6/week6pic1.png)
![week6pic2](https://github.com/stellaczh/Mechatronics/blob/master/week6/week6pic2.GIF)
![week6pic3](https://github.com/stellaczh/Mechatronics/blob/master/week6/week6pic3.GIF)

code;
const int analogInPin = A0;  // Analog input pin that the potentiometer is attached to
const int analogOutPin = 3; // Analog output pin that the LED is attached to

int sensorValue = 0;        // value read from the pot
int outputValue = 0;        // value output to the PWM (analog out)

void setup() {
  // initialize serial communications at 9600 bps:
  Serial.begin(9600);
  // declare pin 3 to be an output:
  pinMode(analogOutPin, OUTPUT);
}

void loop() {
  // read the analog in value:
  sensorValue = analogRead(analogInPin);
  // map it to the range of the analog out:
  outputValue = map(sensorValue, 0, 1023, 0, 255);
  // change the analog out value:
  //analogWrite(analogOutPin, outputValue);

  // print the results to the Serial Monitor:
  Serial.print("sensor = ");
  Serial.print(sensorValue);
  Serial.print("\t output = ");
  Serial.println(outputValue);

   if (sensorValue <= 600) {
    analogWrite(analogOutPin,0);
  }

  if (sensorValue >= 600) {
    analogWrite(analogOutPin, outputValue*10);
  }

  // wait 2 milliseconds before the next loop for the analog-to-digital
  // converter to settle after the last reading:
  delay(2);
}


# week 7-8
For this electrocar midterm project, I teamed up with Rio to make a electrocar. Rio put the car together and tested the motor, I coded for obstacle avoidance and remote control.
![week7pic1](https://github.com/stellaczh/Mechatronics/blob/master/week7/week7pic1.png)
![week7pic2](https://github.com/stellaczh/Mechatronics/blob/master/week7/week7pic2.JPG)
![week7pic3](https://github.com/stellaczh/Mechatronics/blob/master/week7/week7pic3.JPG)

Obstacle avoidance demo:
![week7pic4](https://github.com/stellaczh/Mechatronics/blob/master/week7/week7pic4.GIF)

Remote control demo:
![week7pic5](https://github.com/stellaczh/Mechatronics/blob/master/week7/week7pic5.GIF)
