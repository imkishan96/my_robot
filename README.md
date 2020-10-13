# Map My World

ROS package for udacity project Map My World
**Note** : rename the folder Where_Am_I to my_robot

## Install

clone the repository `Map_my_world` and **rename** it to `my_robot`.

```
cd catkin_ws/src

mv ~/catkin_ws/src/Where_Am_I ~/catkin_ws/src/my_robot

```

download database file from the link
```
https://drive.google.com/file/d/1TefOGKuQf3E4D545fgo4K_xB70g6LoEr/view?usp=sharing
```
and save the file `map_my_world.db` in the my_robot folder

build and source
```
cd ..
catkin_make
source devel/setup.bash
```
## Launch
launch world.launch file
```
cd catkin_ws
source devel/setup.bash
roslaunch my_robot world.launch
```
on new terminal launch localization.launch file
```
source devel/setup.bash
roslaunch my_robot localization.launch
```
on new third terminal launch teleop.launch
```
source devel/setup.bash
roslaunch my_robot teleop.launch
```