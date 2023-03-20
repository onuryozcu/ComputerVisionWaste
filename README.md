# ComputerVision

It is the completed version of the image processing page of the interface where I carry out computer vision and artificial intelligence projects.

In the continuation of the interface, integration of artificial intelligence projects such as object classification, recognition and segmentation and system communications will be carried out.

- 🚀

# User Interface 

It is the homepage of the interface developed for the integrated operation of the waste separation system with computer vision and artificial intelligence.

- `Home PAGE` - Encoder counts per revolution
- `Image Processing Analysis` - Execution rate of the *Arduino* code (see Arduino side documentation for details)
- `Signal Flow System` - Serial port to connect to (default `/dev/ttyUSB0`)
- `Settings` - Serial baud rate (default `57600`)
- `Data Visualization` - Enables debugging of serial commands (default `false`)



<br>
<br>
<p align="center">
    <img width="1900" src="a1.PNG" alt="system">
</p>


<br>
<br>
<p align="center">
    <img width="1900" src="main.png" alt="system">
</p>




##########################################################333

## Components

The `serial_motor_demo` package consists of two nodes, `driver.py` and `gui.py`. The idea is that the driver can be run on an onboard PC inside a robot (e.g. a Raspberry Pi), interfacing with the lower-level hardware. The driver exposes motor control through ROS topics (see below), which are to be published by the user's software.

The GUI provides a simple interface for development and testing of such a system. It publishes and subscribes to the appropriate topics.


To run, e.g.
```
ros2 run serial_motor_demo driver --ros-args -p encoder_cpr:=3440 -p loop_rate:=30 -p serial_port:=/dev/ttyUSB0 -p baud_rate:=57600
```

It makes use of the following topics
- `motor_command` - Subscribes a `MotorCommand`, in rads/sec for each of the two motors
- `motor_vels` - Publishes a `MotorVels`, motor velocities in rads/sec
- `encoder_vals` - Publishes an `EncoderVals`, raw encoder counts for each motor



## GUI Usage

Has two modes, one for raw PWM input (-255 to 255) and one for closed-loop control. In this mode you must first set the limits for the sliders.


## TODO

- Add service for encoder reset
- Add service for updating PID parameters
- Stability improvements
- More parameterisation



