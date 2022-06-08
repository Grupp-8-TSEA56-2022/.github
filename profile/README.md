# Grupp 8 Taxibil
This is a collection of git repositories created in TSEA56 (Electronics
Engineering - Bachelor Project) course.

![A picture of the car](https://raw.githubusercontent.com/Grupp-8-TSEA56-2022/.github/master/images/taxi.jpg)

In the course an autonomous taxi car was created.
The car uses a camera to take pictures.
Those pictures are then processed on a Raspberry Pi 3 using the openCV library.
There is also 2 AVR-processors (ATMEGA1284P) on the car.
One is used to measure speed and obstacle distances and one to handle the
steering of car.
Those processors are reached through I2C.
The Raspberry Pi itself acts as a TCP socket so that an external laptop can
connect to it and control it.

The most important repositories are:
- communication-module: Contains the main program for the Raspberry Pi. Includes
  many other repositories as git submodules.
- image-processing-module: Contains the code for the image processing module.
- control-center: Contains the code for the control center module. It handles
  autonomous driving logic.
- sensor-module: Runs on ATMEGA1284P. Handles all sensors except for the
  camera.
- steering-module: Runs on ATMEGA1284P. Handles the steering and regulation of
  the car.
- user-interface: Python front-end which allows the user to monitor sensor data
  and control the car.

A lot more information can be found in the documentation. It is however in
Swedish.
