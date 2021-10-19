该文件为在ROS中建立小车模型。

首先配置好环境变量

然后用下列命令启动gazebo
```bash
roslaunch urdf02_gazebo car_gazebo.launch
```

用下列命令启动rviz，可以可视化传感器数据
```bash
roslaunch urdf02_gazebo car_rviz.launch
```

可以运行键盘控制节点控制小车运动
```bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py 
```
