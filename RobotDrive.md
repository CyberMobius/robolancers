RobotDrive class of the WPILib confusions.

The mecanumDrive\_Cartesian and mecanumDrive\_Polar methods are a bit confusing.

Basically, for mecanumDrive\_Cartesian, the parameter x means the speed in the X Axes, y means the speed in the y Axes and rotation means the amount of rotation the robot will spin (Think of arcadeDrive and the x-axis that is plugged in to drive the robot, moving the joystick all the way to the right will produce a value of 1, meaning turn the robot left, vice versa). The angle parameter is optional. However, if you plug it in, it will enable Field Oriented Drive (The robot will move forward according to your point of view of forward/Google this). However, your forward will only drive the robot forward if the robot's forward, when lined up with your forward, is giving a gyro angle of 0.

For mecanumDrive\_Polar, you need some knowledge of how polar graphs/vectors work. The parameter magnitude is the speed, angle dictates the direction the robot will go (polar graph knowledge) and rotation is the same as above. The x and y axes of a joystick can be converted into polar graph measurements/coordinates.

Remember that for the mecanumDrive methods to work, when you initialize your RobotDrive object, you need to have 4 speed controllers initialized. This means that if you only plugin 2 channels or speed controllers into the constructor, the mecanumDrive methods will return a null pointer exception.

If you are experiencing some motors going in the opposite desired directions, you can either
A. Use the setInvertedMotor method
B. Switch the inputs going into the drive methods
C. Rewire the polarity (Not recommended)