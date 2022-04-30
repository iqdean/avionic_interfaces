## Custom ROS Message to publish Euler Angles (Roll Pitch Yaw) read from bno055 sensor

---
### TODO:
Add details on how add this to you ros2 workspace, so you can use the 'RPY' message format in a node

---
### Rough How To
 1257  cd ros2_ws
 1285  ros2 pkg create --build-type ament_cmake cpp_pubsub
 
 1323  ros2 pkg list | grep avionic
 1324  ros2 interface show avionic_interfaces/msg/RPY
