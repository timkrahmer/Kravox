# Kravox
Resources for building a Kravox – A wireless, orientation and touch sensing musical Instrument

Kravox has been created as part of a research project at Lund University (Sweden) with the aim to give digital musical instrument controllers the feeling of conventional, mechanical instruments
Now Kravox shall be made accessible for everyone and serve as a musical experimentation platform, so this detailed tutorial has been created to enable as many people as possible to use this exciting new Instrument!



# How to play Kravox

Playing Kravox is as quite straightforward. Just imagine you are playing around with an ordinary object like a broom and the way you touch and move it through space controls how sound is generated. 



# What is Kravox

Kravox is a cross-platform compatible, digital open source musical instrument that consists of three components – controller/s, receiver and software

Controller/s

Up to three wireless controller devices can be connected. Each controller processes orientation- and acceleration data from a digital mpu6050-gyroscope and touch data from two MPR121-touch-sensor-boards connected to an Arduino Nano. The controller/s send/s the data to a receiver device via NRF24L01 radio transceiver/s. 
If more than one controller shall be used, the second and third controller need to get individual addresses assigned. For more information about assigning the address see the info in the DECLARATIONS / NRF24L01 section of the controller code.

Receiver

The receiver passes the data received from the controller/s on via USB to a connected computer, together with data collected from several potentiometers. The provided receiver device code  allows communication with up to three controllers, but will also work with only one or two without adjustments.

Software

The data from the receiver is processed in a programme written in Pure Data Vanilla that outputs sound.
