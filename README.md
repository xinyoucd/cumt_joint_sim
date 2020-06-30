<center>

# **CUMT_Joint_Simulation**

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<h1 align=center>

<img src="/cumt_sim/image_view/CUMT.png" width="400" height="300" />

<center> CUMT </center>

<img src="/cumt_sim/image_view/sun_2.jpg" width="800" height="150" />

<center>Sunspeed_Robotics</center>

</h1>

- **Annotate：**
  - CUMT **===>**(China University of Mining and Technology)

<center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

## **Project Description**

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- **Explanation：**
  - Use the **bufflo** mobile-robot as the underlying mobile system of the robot system;
  - Use the aubo robotic-arm as a robotic gripping system;
  - Building a co-simulation model;
  - Show in **rviz** debugging environment;

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- Robot_image_view
  - **Bufflo-robot-view**
  
  <center>

  <img src="/cumt_sim/image_view/bufflo.png" width="400" height="350" />

  </center>

  - **Aubo_robot_view**

<center>

  <img src="/cumt_sim/image_view/aubo_robotics.jpg" width="400" height="350" />

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<center>

## Model Description

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<center>

```mermaid
graph TD
A[driver_link]-->B1(joint_pedestal)
A[driver_link]-->B2(joint_radar)
A[driver_link]-->B3(joint_pedestal)
B1(joint_pedestal)-->C1[pedestal_link]
B2(joint_radar)-->C2[radar_link]
B3(joint_support)-->C3[support_frame_link]
C3[support_frame_link]-->D(joint_wind)
D(joint_wind)-->E[wind_vane_link]
```

</center>

<center>

**Bufflo_robot_link_description**

</center>

- **Robot-Description**
  - **General Description:**
    - **Link** description of the **bufllo** robot overall:
      - **driver_link**
      - **pedestal_Link**
      - **radar_link**
      - **support_frame_Link**
      - **wind_vane_Link**
    - **Joint_Link** description of the **bufflo** robot overall:
      - **pedestal_joint**
      - **radar_joint**
      - **support_frame_joint**
      - **wind_joint**
- **Aubo_robot_arm**-description
  - Read the official documentation;
  - You can visit the following URL
    - <http://www.aubo-robotics.cn/>
    - <http://wiki.ros.org/aubo_robot>
    - <https://github.com/lg609/aubo_robot>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<center>

## Test Environment

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- System version:
  - ubuntu 16.04 (Xenial Xerus)

<center>

<img src="/cumt_sim/image_view/11.jpeg" width="300" height="180" />

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- ROS version:
  - rosdistro: kinetic
  - rosversion: 1.12.14

<center>

<img src="/cumt_sim/image_view/kinetic.png" width="400" height="350" />

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- **Explanation**
  - If you want to try other environments, it is basically possible. If the debugging is successful, you can post your test results in the comment area.
  - Love you.
  - I hope you enjoy your day!
  - :kissing_heart: :kissing_heart:  :kissing_heart:

<center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

## How to run this package

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

</center>

- **Compile and start**

```bash
mkdir -p text_ws/src
cd text_ws/src
catkin_init_workspeace
```

- put **cumt_joint_sim** package in you create workspeace/src

```bash
cd .. && catkin_make
source devel/setup.bash
roslaunch aubo_i5_moveit_config moveit_planning_execution.launch robot_ip:=127.0.0.1
```

- open new terminal **(ctrl + alt + t)**

```bash
source ~/catkin_ws/devel/setup.bash
roslaunch aubo_gazebo aubo_i5_gazebo_control.launch
```

- Not surprisingly, after subscribing to related ROS topics, you will see the model of co-simulation;
- Note :
  - text_ws is a test workspace I named
  - You can also use your own name
  
<center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

## **Maybe needed dependency**

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- Install the following packages

```bash
sudo apt-get install ros-kinetic-moveit*
sudo apt-get install ros-kinetic-gazebo-*
sudo apt-get install ros-kinetic-joint*
sudo apt-get install ros-kinetic-ros-*
```

- There are other problems
  - you can visit **ros_wiki**;
  - you can visit **google**;
- The best solution
  - contact the relevant salesperson;
  - looking forward to your call;

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<center>

## Show_Results

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<center>

<img src="/cumt_sim/image_view/Rviz_joint_sim.png" width= "900" height="507" />

<img src="/cumt_sim/image_view/gazebo_joint_sim.png" width= "900" height="507" />

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<center>

## Last

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- Please enjoy this model！
- :joy: :joy: :joy:

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

<center>

## Statement

</center>

<center>

<img src="/cumt_sim/image_view/title_3.png" width= "1000" height="60" />

</center>

- I declare here:
  - This package is just for my casual construction, it has no practical significance;
  - I have written the complete package and handed it to the client, so I cannot share it with you;
