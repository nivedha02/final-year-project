# IR SENSOR

Infrared technology addresses a wide variety of wireless applications. The main areas are sensing and remote controls.
In the electromagnetic spectrum, the infrared portion is divided into three regions: near infrared region, mid infrared region and far infrared region.

![irsensor](https://hackster.imgix.net/uploads/attachments/1173102/image_rLAOUdKU7s.png?auto=compress%2Cformat&w=1280&h=960&fit=max)

Infrared technology addresses a wide variety of wireless applications. The main areas are sensing and remote controls. 
In the electromagnetic spectrum, the infrared portion is divided into three regions: 
near infrared region, mid infrared region and far infrared region.

![description](https://hackster.imgix.net/uploads/attachments/1173104/image_5M80I7XDgg.png?auto=compress%2Cformat&w=1280&h=960&fit=max)

The wavelengths of these regions and their applications are shown below.

Near infrared region — 700 nm to 1400 nm — IR sensors, fiber optic
Mid infrared region — 1400 nm to 3000 nm — Heat sensing
Far infrared region — 3000 nm to 1 mm — Thermal imaging
The frequency range of infrared is higher than microwave and lesser than visible light.

For optical sensing and optical communication, photo optics technologies are used in the near infrared region as the light is less complex than RF when implemented as a source of signal. 
Optical wireless communication is done with IR data transmission for short range applications.

An infrared sensor emits and/or detects infrared radiation to sense its surroundings.

The working of any Infrared sensor is governed by three laws: Planck’s Radiation law, Stephen – Boltzmann law and Wien’s Displacement law.

Planck’s law states that “every object emits radiation at a temperature not equal to 00K”. Stephen – Boltzmann law states that “at all wavelengths, the total energy emitted by a black body is proportional to the fourth power of the absolute temperature”. According to Wien’s Displacement law, “the radiation curve of a black body for different temperatures will reach its peak at a wavelength inversely proportional to the temperature”.

The basic concept of an Infrared Sensor which is used as Obstacle detector is to transmit an infrared signal, this infrared signal bounces from the surface of an object and the signal is received at the infrared receiver.

![des](https://hackster.imgix.net/uploads/attachments/1173105/image_Moyca67CUH.png?auto=compress%2Cformat&w=680&h=510&fit=max)

### Stimulation

![screenshot_(25)_c3VF7VzPev](https://user-images.githubusercontent.com/76787422/157839102-c4cc5bac-d3ff-42e7-9ae3-571118a910dd.png)

### CODE
```
void setup()
{
  pinMode(13,OUTPUT);//led
  pinMode(3,INPUT); //ir sensor
  Serial.begin(9600);
}
void loop()
{
  if (digitalRead(3)== LOW) //if no heat
  {
    digitalWrite(13,HIGH);
    
    delay(10);
  }
  else 
  {
    
    digitalWrite(13,LOW);
    delay(10);
    
  }
  
}

```

### OUTPUT

If the heat reaches the ir sensor,then the led glows.



