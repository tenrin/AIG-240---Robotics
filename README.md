Project 1 – Setting up ROS 2 and Gazebo

Group 7 : Nima Arabi, Ledi Caushi, Yuliya Dubovichenko, Tenzin Rinchen
Questions

1. What command did you use to create a ROS 2 package?
2. Explain why and how you used ROS messages in your program.
3. How do you verify that your ROS 2 node is publishing messages correctly?
4. Describe the steps to launch Gazebo and your ROS 2 node simultaneously.


Answers:

1. For creating a ROS 2 package, we use the below command:
    ros2 pkg create package_name

2. We use ROS messages in the program to communicate with different nodes in the ROS2 system. ROS Messages are used to transmit data between the publishers and subscribers.

3. To verify that my ROS 2 node is publishing messages correctly, We used the ros2 topic echo command.

4. To launch Gazebo and my ROS 2 node simultaneously, I follow these steps:
	• Make sure Gazebo is installed along with ROS2
	• Create a launch configuration gor both Gazebo and ROS2 node.
	• Launch file contains necessary launch descriptions for initializing Gazebo with desired world and configurations.
	• Include Description for starting ROS2 node and specify the parameters.
	• Execute the launch file using ROS2 launch command. This launcher would contain both Gazebo and ROS 2 node simultaneously
	• In a terminal run this code:
    	◦ ros2 run turtlesim turtlesim_node
	• Open another terminal and run this code simultaneously:
    	◦ ros2 run turtlesim turtle_teleop_key
