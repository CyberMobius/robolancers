The ADXL345 accelerometer was received in the 2012 FRC KOP and in one other year previously.

The sensor board also included a gyro. These two sensors are able to be separated. They do not require each other for their operations.

The ADXL345 is able to communicate to the cRIO through two ways. Using I2C protocol or something else (TODO Find out what it was and fill this in guys...). Check out LabVIEW examples for wiring diagrams.

However, so far, the method I have tried (Eric) was I2C and it did not work in any of my test. Through further research, I have found that for some reason, the cable from the Digital Sidecar to the Digital Module on the cRIO affects it. Apparently, using the old D37 cable does not work. What does work though are the new D37 Ribbon Cables which come in the FRC KOPs now. However I broke the 2012 one (Eric) so as of 4/14/2012, we do not have one.