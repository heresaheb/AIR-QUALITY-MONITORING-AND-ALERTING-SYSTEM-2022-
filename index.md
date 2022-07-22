
# AIR QUALITY MONITORING AND ALERTING SYSTEM (2022)



## Abstract-
Air pollution affects our day to day activities and quality of
life. It poses a threat to the ecosystem and the quality of life on the
planet. The dire need to monitor air quality is very glaring, owing to
increased industrial activities over the past years. People need to
know the extent to which their activities affect air quality. This
project proposes an air pollution monitoring system. The system was
developed using the Arduino microcontroller and MQ135 air quality
sensor. The air pollution monitoring system was designed to monitor
and analyze air quality in real-time. Air quality measurements were
taken based on the Parts per Million (PPM) metrics and analyzed
using Microsoft Excel. The air quality measurements taken by the
designed system was accurate. The result was displayed on the serial
monitor of the arduino IDLE.
## Authors

- [Subhajit Basak (11705518048)](https://www.linkedin.com/in/subhajit21/)
- [Ayan Saha (11705518039)](https://www.linkedin.com/in/ayan-saha-050422218/)
- [Aritro Ghosh (11705518041)](https://www.linkedin.com/in/aritro-ghosh-242305212/)
## Under Supervision of
[Mr. Kalyan Biswas](https://www.linkedin.com/in/kalyan-biswas-921b8635/)
-> Assistant Professor

Applied Electronics and Instrumentation
Engineering Branch

RCC Institute of Information Technology
## Components
1. Arduino UNO
2. MQ135 sensor
3. Buzzer
4. LED
5. Jumper wires
## ARDUINO CODE
```
{
int a=0;

void setup()

{

  pinMode(8,OUTPUT);   // to set up all the pins
  
  pinMode(A1, INPUT);
  
  pinMode(7,OUTPUT);
  
  Serial.begin(9600); // Baude rate
 
 }

void loop()

{

  int val=analogRead(A1);

  if (a==0)

  {

   Serial.println(val);

   a=a+1;

   }

  if (a!=0)
  
  {
   
    if(val>200)
  {
       
    Serial.println(val);
    digitalWrite(8,HIGH);
    digitalWrite(7,HIGH);
    delay(500);
    digitalWrite(7,LOW);
   }
   }
}
}
```

## Published By

**2022 IEEE Calcutta Conference (CALCON)**


**For More** 
- [Click here](https://drive.google.com/drive/folders/1aH3e5B0goLYNwEz7WpyysoAaFcEurzs4?usp=sharing)
