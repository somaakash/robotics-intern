# robotics-intern

commands to be used:- 

  cd ros2_ws
  
  colcon build --symlink-install
  
  source install/setup.bash
  
  ros2 launch my_robot_bringup my_robot_gazebo.launch.xml

  ros2 topic list
  
  ros2 topic info /cmd_vel
  
  ros2 interface show geometry_msgs/msg/Twist
  



to move the robot :-straight

   ros2 topic pub /cmd_vel geometry_msgs/Twist "{linear: {x: 0.5}, angular:{z: 0}}"
   
to move the robot :-straight and angularly

  ros2 topic pub /cmd_vel geometry_msgs/Twist "{linear: {x: 0.5}, angular:{z: 0.1}}"
  
to stop the robot:

  ros2 topic pub /cmd_vel geometry_msgs/Twist "{linear: {x: 0}, angular:{z: 0}}"







