
# aerial_project
Eurecat UVIC master repository for final aerial project



## How to set up the project framework

### Install catkin tools

    wget http://packages.ros.org/ros.key -O - | sudo apt-key add -
    sudo apt-get install python-catkin-tools

### Install vcstool

    sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
    sudo apt-key adv --keyserver hkp://pool.sks-keyservers.net --recv-key 0xAB17C654
    sudo apt-get update
    sudo apt-get install python3-vcstool


### Ros packages (Maybe not complete)
Install ros packages

    sudo apt-get install ros-${ROS_DISTRO}-lms1xx
    sudo apt-get install ros-${ROS_DISTRO}-controller-manager
    sudo apt-get install ros-${ROS_DISTRO}-base-local-planner
    sudo apt-get install ros-${ROS_DISTRO}-dwa-local-planner  
    sudo apt-get install ros-${ROS_DISTRO}-joint-state-controller  
    sudo apt-get install ros-${ROS_DISTRO}-gazebo-ros-control  
    sudo apt-get install ros-${ROS_DISTRO}-diff-drive-controller  
    sudo apt-get install ros-${ROS_DISTRO}-move-base
    sudo apt-get install ros-${ROS_DISTRO}-twist-mux
    sudo apt-get install ros-${ROS_DISTRO}-clear-costmap-recovery
    sudo apt-get install ros-${ROS_DISTRO}-nav-core
    sudo apt-get install ros-${ROS_DISTRO}-navfn
    sudo apt-get install ros-${ROS_DISTRO}-rotate-recovery
    sudo apt-get install ros-${ROS_DISTRO}-octomap
    sudo apt-get install ros-${ROS_DISTRO}-octomap-ros
    sudo apt-get install ros-${ROS_DISTRO}>-octomap-msgs
    sudo apt-get install ros-${ROS_DISTRO}-geographic-msgs
    sudo apt-get install ros-${ROS_DISTRO}-mavlink
    sudo apt-get install ros-${ROS_DISTRO}-robot-localization
    
    sudo apt-get install libgeographic-dev
    sudo apt-get install libgoogle-glog-dev
    pip install future


###  ROS kinetic (and ubuntu 16.04 LTS):

Get the vcs repo file:

    wget https://raw.githubusercontent.com/AerialRobots/aerial_project/master/project_cfg/vcsFiles/kinetic.repos

Import the repos

    vcs import < kinetic.repos

Run the python script located in 

    python3 aerial_project/project_cfg/scripts/kineticUpdates.py


### Ros melodic (and ubuntu 18.04 LTS):

Get the vcs repo file:

    wget https://raw.githubusercontent.com/AerialRobots/aerial_project/master/project_cfg/vcsFiles/melodic.repos

Import the repos

    vcs import < melodic.repos

Run the python script located in 

    python3 aerial_project/project_cfg/scripts/melodicUpdates.py

### Compile everything

Inside the workspace folder run:

    catkin build






