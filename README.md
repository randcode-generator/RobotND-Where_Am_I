# RobotND - Where Am I

This is the third project for the Udacity [Robotics Software Engineer](https://www.udacity.com/course/robotics-software-engineer--nd209) course. The objective of this project is to find the best parameters to localize our robot. 

Initial localization
![](images/image1.png 'image1')

Localized after rotating using teleop
![](images/image2.png 'image2')

## How to build
```
mkdir -p catkin_ws/src
cd catkin_ws
cp -r ../RobotND-Where_Am_I/* src/
catkin_make
```

## How to run
Open a terminal and run the following
```
cd <path to catkin>/catkin_ws/
source devel/setup.bash
roslaunch my_robot world.launch
```

Open a new terminal and run the following
```
cd <path to catkin>/catkin_ws/
source devel/setup.bash
roslaunch my_robot amcl.launch
```

Open a new terminal and run the following
```
cd <path to catkin>/catkin_ws/
source devel/setup.bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```