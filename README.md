## Custom ROS Message to publish Euler Angles (Roll Pitch Yaw) read from bno055 sensor

---
### TODO:
Add details on how add this to you ros2 workspace, so you can use the 'RPY' message format in a node

---
### Rough HowTo's
```
 1257  cd ros2_ws
 1308  ros2 pkg create --build-type ament_cmake avionic_interfaces
 ...
 1323  ros2 pkg list | grep avionic
 1324  ros2 interface show avionic_interfaces/msg/RPY

iqdean@rpi3ubu2004:~/ros2_ws$ ros2 pkg list | grep avionic
avionic_interfaces
iqdean@rpi3ubu2004:~/ros2_ws$ colcon build --packages-select avionic_interfaces
```
```
NOTE:
iqdean@rpi3ubu2004:~/ros2_ws/src/avionic_interfaces$ tree
.
├── CMakeLists.txt
├── include
│   └── avionic_interfaces  < empty, must be build artifact
├── msg
│   └── RPY.msg
├── package.xml
├── README.md
└── src                     < empty, must be build artifact

```
