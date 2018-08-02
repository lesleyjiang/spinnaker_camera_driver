# spinnaker_camera_driver
To run the drivers, when run the code:
```bash
roslaunch acquisition.launch
```
An error "No cameras found!" occurred due to the failure of USB recognition. To solve this, go to the spinnaker source code directory and run the code:
```bash
sudo ./spin-conf
```
Follow the instructions and reboot the device. Then run ``` roslaunch acquisition.launch ``` .
