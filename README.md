# Mini_Project_1

Group 2:
Alan Lacerda
Daniel Smith
Nickson Dos Santos

This project is our submission for the mini-project 1. The goal is to have a robot seek out a light source and move to it using a light sensor.
Our code uses only one light sensor instead of two. A few functions such as the reading() and drive() were based on the test programs used in class.
The propriety functions created are turn() and self_correct(). Self_correct() has the robot turn to seek out the general direction of the light source.
Once the source is found, the robot will then move in that direction. The robot will constantly take measurements from its light sensor as it drives. 
If it determines that the readings begin to decrease, it will then begin to turn to find the light source again. Turn() gives instructions on how to turn, the robot will take an initial reading that it stopped moving on. It will use this value to determine whether or not to continue turning. Measurments will also be taken throughout this function.
The robot will initially turn right and will continue to turn right until the readings decrease. Once the readings decrease, the robot will turn left to find higher readings. 
The robot will continue this loop of right and left turns until it finds a reading that is within a certain range of the reading it initially stopped on.

This code works decently, the robot does seek out a light source and will turn to find it. However, it often targets the light reflected of walls as well as light coming
through windows. Additionally, the robot begins to turn at a reduced angle the longer it is stuck in a loop. Another goal was to stop when the robot records a certain reading.
Unfortunately, this was not implemented due to time constraints and not knowing how best to go about this.
