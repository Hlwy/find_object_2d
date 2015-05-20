## find-object (standalone)
Find-Object project, visit the [home page](http://introlab.github.io/find-object/) for more information.

## find_object_2d (ROS package)

### Install
```bash
# Install ROS Groovy/Hydro/Indigo/Jade (catkin build):
 $ cd ~/catkin_ws
 $ git clone -b find_object_2d https://github.com/introlab/find-object.git src/find_object_2d
 $ catkin_make

# Install ROS Fuerte (in a directory of your "ROS_PACKAGE_PATH"):
 $ svn checkout -r176 http://find-object.googlecode.com/svn/trunk/ros-pkg/find_object_2d
 $ rosmake find_object_2d
```

### Run
```bash
 $ roscore &
 # Launch your preferred ubs camera driver
 $ rosrun uvc_camera uvc_camera_node &
 $ rosrun find_object_2d find_object_2d image:=image_raw
```
See [find_object_2d](http://wiki.ros.org/find_object_2d) for more information.