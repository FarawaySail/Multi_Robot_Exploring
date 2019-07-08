# Multi_Robot_Exploring
## Environment
- ROS
- Gazebo
- ORB-SLAM

## Contribution
- Multi-Robot
- Use RGB-D not LiDAR
- Exploring and mapping

## Already do
- ORB-SLAM2 
- Place two robots

## To do
- Get ORB-SLAM2's pose information and corresponding depth map
- Transform pose and map to point cloud
- mapping
- ...

## Remarks
- 深度图实际上是OpenCV类型为32FC1的Mat。其中每个数是$0~10$的浮点数。当使用`rostopic echo /camera/depth/image_raw`时，表面上输出为$0~255$的整数，实际上得把三个数连起来看才可以。具体可以参考image_view函数，或者通过rviz仿真，改变Normalize Range来观察。
