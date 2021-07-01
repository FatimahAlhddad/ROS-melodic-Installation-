# ROS-melodic-Installation-
After running VM with ubuntu 18.04 OS, this steps for install ROS melodic 

## 1- Setup sources.list
`$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`

## 2- Set up keys
`$ curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -`

## 3- Installation
`$ sudo apt update`</br>
Desktop-Full Install:</br>
`$ sudo apt install ros-melodic-desktop-full`

## 4- Initialize rosdep
`$ sudo apt install python-rosdep`</br>
`$ rosdep update`

## 5- Environment setup
`$ echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc`</br>
`$ source ~/.bashrc`

## 6- Dependencies 
`$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential`</br>


# Preparing ROS
Create a workspace by using catkin_make</br>
`$ mkdir -p ~/catkin_ws/src`</br>
`$ cd ~/catkin_ws/`</br>
`$ catkin_make`</br>
`$ echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc`</br>
`$ source ~/.bashrc`</br>


## Result:
`$ roscore`</br>
![image](https://user-images.githubusercontent.com/85858256/124070847-239da800-da47-11eb-892e-65ae926011cd.png)
