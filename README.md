## Localizing a Mobile Robot Using ROS

![68747470733a2f2f73332d75732d776573742d312e616d617a6f6e6177732e636f6d2f756461636974792d726f626f746963732f45787472612b496d616765732f526f626f4e445f666c61672e706e67](https://user-images.githubusercontent.com/20925510/33958665-1e55e9c8-e056-11e7-9711-d21b9f681de6.png)

A mobile robot with a laser rangefinder and camera is localized in the RViz and Gazebo simulation environments with the help of ROS packages. Adaptive Monte Carlo Localization (AMCL) and navigation stack packages are used in this project. Detailed information is available on the [write-up](https://github.com/bahadirozkan/whereAmIRobot/blob/master/localizing-mobile-robot.pdf) document.

To launch the project and test it on the RViz and Gazebo environments, first go to the catkin workspace directory and source it.
```
$ cd ~/catkin_ws/
$ source devel/setup.bash
```
Then launch the nodes with the following commands on seperate terminals. 
```
$ roslaunch udacity_bot mod_udacity_world.launch
$ roslaunch udacity_bot amcl_mod.launch
```
You will see something similar to this:

![readme1](https://user-images.githubusercontent.com/20925510/39756336-d91aa5b2-52d1-11e8-83be-a8f1016bb6db.JPG)

If not, check your project repository. 
If everything's fine then on a seperate terminal run the command below to send the robot to the goal position. 
```
$ rosrun udacity_bot navigation_goal
```
Robot should reach the goal position after some time!

You can find the images of classroom and modified robots' at the goal position:
+ [Udacity robot](https://github.com/bahadirozkan/whereAmIRobot/blob/master/udacity_bot%20goal.JPG)
+ [Modified robot](https://github.com/bahadirozkan/whereAmIRobot/blob/master/mod_bot%20goal.JPG)
