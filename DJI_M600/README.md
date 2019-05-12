# How to access the manifold?
IP address of the Manifold on DJI M600 192.168.1.100 so if you connect your computer to the router on DJI M600, you can set your ip as 192.168.1.110 and make an ssh connection to manifold by running the command below:

ssh ubuntu@192.168.1.100

# Why manifold is not at the upper side of the M600?
Because manifold affects GPS sensors badly.

# How to install DJI OSDK ?
- Open a terminal, cd into the onboardsdk folder and follow these steps to build the core OSDK library
> mkdir build

> cd build 

> cmake .. && make djiosdk-core && sudo make install djiosdk-core

# Which version to use?
It was not possible to use RTK GPS with Version 3.7 so I used Version 3.6


# How to use DJI with ROS?
Download https://github.com/dji-sdk/Onboard-SDK-ROS and catkin make the packages in a catkin workspace. You can also use enc_key and app_id in the sdk.launch file. 
