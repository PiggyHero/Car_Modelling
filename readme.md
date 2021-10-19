该文件为在ROS中建立小车模型。

首先配置好环境变量

# 1 创建小车模型及传感器并在gazebo和rviz中显示
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
# 2 slam建图
先运行下列命令启动gazebo并导入小车模型
```bash
roslaunch urdf02_gazebo car_gazebo.launch
```
然后运行

```bash
roslaunch navigation_demo nav01_slam
```

完成slam建图