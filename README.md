# YOLO-ROS

**YOLO-ROS for NVIDIA**

**YOLO-ROS for HUAWEI ATLAS200, please checkout for branch `atlas200`**

Modified from [ros-yolov5](https://github.com/OuyangJunyuan/ros-yolov5), originated from [yolov5](https://github.com/ultralytics/yolov5)

1. clone `YOLO-ROS`
   ```
   cd {YOUR_WORKSPACE}/src
   git clone https://github.com/jianhengLiu/yolo_ros.git
   ```

2. install python dependencies
```
   sudo apt install ros-melodic-ros-numpy
   pip3 install --upgrade pip
   pip3 install -r yolo_ros/requirements.txt`
```
3. `catkin_make`

4. `roslaunch yolo_ros yolo_service.launch`

5. play your rosbag.

## Possible problem

catkin error: 
`yolo_ros/src/service_client.cpp:19:10: fatal error: yolo_ros/yolo.h: No such file or directory`

Just run `catkin_make` a second time.