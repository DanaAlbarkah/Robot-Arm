# Install and Run robot-arm package on ROS  
First you have to folow the following steps if you do not have a Linux Distribution:  
  1- install VMware using the following link:   
    https://my.vmware.com/en/web/vmware/downloads/details?downloadGroup=WKST-PLAYER-1612&productId=1039&rPId=66621  
  2- install ubuntu using the following link ( I use ubuntu 16.04)  
    https://releases.ubuntu.com/16.04/  
  3- inside the VMware creat a new virtual machine and put your ubuntu file in it   
  4-run your ubutu   

## Inside ubutu:
1- open a new terminal  
2- open  s-m.com.sa/ros.txt  
3- copy and paste each line using the previous link and run it in the terminal when you are done it should look like this:  
![image](https://user-images.githubusercontent.com/85397914/123515664-f6e13d80-d6a0-11eb-97ff-a95a885602dd.png)  

## Opening gazebo:  
Here we gonna need four terminals :  
1- write the following code in the first terminal and the arm  should appear in Rvize:  
  roslaunch robot_arm_pkg check_motors.launch  
2- write the following code in the second terminal and the arm should appear in gazebo:  
  roslaunch robot_arm_pkg check_motors_gazebo.launch  
3- in the third terminal Write the following code  :  
   cd catkin_ws/src/arduino_robot_arm/robot_arm_pkg/scripts  
   sudo chmod +x joint_states_to_gazebo.py  
4- in the last terminal write this command to control bothe arms in Rvize and gazebo at once:  
    rosrun robot_arm_pkg check_motors_gazebo.launch  
    

https://user-images.githubusercontent.com/85397914/123516909-36128d00-d6a7-11eb-90ae-5ca08491241c.mp4



