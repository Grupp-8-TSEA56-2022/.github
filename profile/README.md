# Grupp 8 Taxibil
This is a collection of git repositories created in TSEA56 (Electronics
Engineering - Bachelor Project) course.

![A picture of the car](https://raw.githubusercontent.com/Grupp-8-TSEA56-2022/.github/master/images/taxi.jpg)

![test](.github/images/taxi.jpg)

In the course an autonomus taxi car was created. 
The car uses a camera to take pictures.
Those pictures are then processed on a Raspberry Pi 3 using the openCV library.
There is also 2 AVR-processors (ATMEGA1284P) on the car.
One is used to measure speed and obstacle distances and one to handle the
steering of car.
Those processors are reached through I2C.
The Rasperry Pi itself acts as a TCP socket so that an external laptop can
connect to it and controll it.
