
## Installing spinnaker_camera_driver
These are some tips for running the FLIR cameras that use the Spinnaker SDK. It has been tested with the Point Grey Blackfly S cameras. 

Before you run the drivers, make sure to add this line to your ``` ./bashrc```:
```bash
source spinnaker_ws/devel/setup.bash
```
To run the drivers, when run the command:
```bash
roslaunch acquisition.launch
```
An error "No cameras found!" may occur due to the failure of USB recognition. To solve this, go to the spinnaker source code directory, configure udev rules to allow access to USB devices and run the following command in the terminal:
```bash
sudo sh spin-conf
```
Follow the instructions and reboot the device. Then run: ```roslaunch acquisition.launch ``` 
