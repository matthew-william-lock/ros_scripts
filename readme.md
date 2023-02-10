# ros_scripts

A collection of tools and scripts for working with ROS.

## Getting Started

1. Clone this repository into your catkin workspace and clone submodules:

```bash
git clone --recurse-submodules https://github.com/matthew-william-lock/ros_scripts
```

# Scripts

### Installing ROS Melodic on Ubuntu 18.04

```bash
cd scripts
sudo chmod +x install_ros_melodic.sh
./install_ros_melodic.sh
```

This will also create some useful aliases for working with ROS. 

| Alias Command | Description |
| --- | --- |
| `eb` | Opens the `~/.bashrc` file for editing using the `nano` text editor. |
| `sb` | Sources the `~/.bashrc` file to reload the environment variables and aliases. |
| `gs` | Runs the `git status` command to check the status of a Git repository. |
| `gp` | Runs the `git pull` command to pull the latest changes from a remote Git repository. |
| `cw` | Changes the current working directory to the `$name_catkin_workspace` folder. |
| `cs` | Changes the current working directory to the `src` folder within the `$name_catkin_workspace` folder. |
| `cm` | Changes the current working directory to the `$name_catkin_workspace` folder and runs the `catkin_make` command to build a ROS package. |

# Commands

## Creating a Catkin Package

Full documentation for creating a catkin package can be found [here](http://wiki.ros.org/ROS/Tutorials/CreatingPackage).

```bash
cd ~/catkin_ws/src
catkin_create_pkg <pkg_name>  std_msgs rospy roscpp
```

> This will create a <pkg_name> folder which contains a package.xml and a CMakeLists.txt, which have been partially filled out with the information you gave catkin_create_pkg.
