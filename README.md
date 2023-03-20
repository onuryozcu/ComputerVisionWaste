# ComputerVision

It is the completed version of the image processing page of the interface where I carry out computer vision and artificial intelligence projects.

In the continuation of the interface, integration of artificial intelligence projects such as object classification, recognition and segmentation and system communications will be carried out.

- 🚀

# User Interface 

It is the homepage of the interface developed for the integrated operation of the waste separation system with computer vision and artificial intelligence.

- `Home PAGE` - The page where the camera *tracking* and *detection* processes are followed.
- `Image Processing Analysis` - The page where *dimensional measurement and image processing analyzes* are made on the detected products.
- `Signal Flow System` - The page where the connection status checks of the camera and other devices are made.
- `Settings` - Settings page, the page where the connection settings are changed.
- `Data Visualization` - Data page, daily tracking and reporting of detected ones.



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



To run, e.g.
```
ros2 run serial_motor_demo driver --ros-args -p encoder_cpr:=3440 -p loop_rate:=30 -p serial_port:=/dev/ttyUSB0 -p baud_rate:=57600
```


## TODO

- Add service for encoder reset
- Add service for updating PID parameters
- Stability improvements
- More parameterisation



