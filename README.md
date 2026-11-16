How to use a photoresistor with Arduino. In this case I have chosen an Arduino Micro.
In my circuit, the photoresistor comes first, followed by a resistor (R1, 10kOhm) in series.
Arduino reads the the voltage drop on R1. Increasing ambient light, photoresistance value decreases, so the microcontroller reads a higher value (voltage drop on R1).
The reading pin is A0. It's an analog pin, so the value gos from 0 to 1023. In the code, we set the range to 0 to 5.
Finally, the photoValue in available by reading on serial monitor.
