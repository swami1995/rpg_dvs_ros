rpg_dvs_ros
===========

ROS packages for the Dynamic Vision Sensor (DVS).  
Find out more on the website of the [Institute of Neuroinformatics](http://siliconretina.ini.uzh.ch/wiki/index.php).

# Driver installation
Make sure, libusb is installed on your system:  
1. `$ sudo apt-get install libusb-1.0-0-dev`

Only a udev rule is needed to run the DVS driver. An install script is provided in the package dvs_driver.  
2. `$ roscd dvs_driver`  
3. `$ ./install.sh` (needs root privileges)

You can test the installation by running a provided launch file. It starts the driver, the renderer, an image viewer, and the dynamic reconfigure GUI.  
4. `$ roslaunch dvs_renderer dvs.launch`  
