# carlike_robot_sim  
Ackermann 转向机构的ROS机器人建图导航与仿真  
  
https://blog.csdn.net/qq_36754438/article/details/109125320  
  
## 准备工作  
### 1、下载代码并安装必要功能包  

环境：  
  
Ubuntu16.04 + ros kinetic  

记得预先安装以下功能包（可能有遗漏，大家根据报错自行安装吧，或者私聊我）   

sudo apt-get install ros-kinetic-ackermann-msgs  
sudo apt-get install ros-kinetic-navigation  
sudo apt-get install ros-kinetic-openslam-gmapping  
sudo apt-get install ros-kinetic-geographic-info  
sudo apt-get install ros-kinetic-controller-manager  
sudo apt-get install ros-kinetic-gazebo-ros-control  
sudo apt-get install ros-kinetic-effort-controllers  
sudo apt-get install ros-kinetic-joint-state-controller   
sudo apt-get install ros-kinetic-position-controllers   
sudo apt-get install ros-kinetic-teb-local-planner  

### 2、编译  
将代码放到自己的工作空间里的src编译（应该不会报错）;  


终端输入:  
cd  
cd catkin_ws  
catkin_make  

## 3.注意！！！在Ubuntu18.04 melodic 版本需要将

PLUGINLIB_DECLARE_CLASS(router, RouterNode, RouterNode, nodelet::Nodelet); 改为 PLUGINLIB_EXPORT_CLASS(RouterNode, nodelet::Nodelet);




