# CameraCalibration_System

OpenCV camera calibration project
Make sure you have a working camera and opencv >= 2.4.x installed.
You just need to print out the chess_pattern.png (images), 
edit the camera_conf.xml (data) according to your needs, build the 
software and execute it. There you go... 

Install and Use
================
```
mkdir build

cd build

cmake ..

make
```
- edit the data/camera_conf.xml to your needs (chess board size, maker size, camera input [0|1 device name])
   Hint: Use a measurer :)
```
cd bin
./cam_calib ../../data/camera_conf.xml
```
- If your camera cannot be found, edit the camera_conf.xml (i.e. change video device index /dev/videoX)

- If your camera is working you will get an image stream indicating "press g to start"

- When done, exit the calibration routine and you will find a calibration xml file next to the executable
