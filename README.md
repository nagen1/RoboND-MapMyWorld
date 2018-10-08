# RoboND-MapMyWorld

RTAB-Map is the best solution for SLAM and robot mapping the 3D environment as the packages is robust in speed, memory management, custom developed tools for easy debug and information analysis tools. Using rtabmap_ros package with ROS wrapper APIs it's ease to build 3D maps for this project. Primarily the RTAB-Map gives the ability to add and use 2D laser, Odometry and RGB-D sensor for mapping. However, for this project we are going to use RGB-D sensor (kinect) as we can use images, depthimage data, laser scan feed,  Odometry for navigation purpose. 


### Challenges/Project Tasks 
#### 1. 2D and 3D mapping for supplied environment
#### 2. Build own environment and generate 2D, 3D maps

### Background
In order to make an autonomous 3D mapping solution, the problem was divided into three parts: (1) the Simultaneous Localization and Mapping (SLAM) that will allow the robot to be aware of its surroundings and it’s location while it moves, the 3D mapping algorithm that takes the sensor data to make a 3D model of the environment,the algorithm that operates the robot to navigate the environment avoiding any obstacles and to get all the necessary data without human intervention. There are many implementations of 2D SLAM and 3D mapping robots with different sensor configurations. The vast majority of hardware configurations employs a dedicated sensor for 2D SLAM, along with other sensors used to gather3D data. By using 3D motion planning (6 DOF), we definitely need a 3D map to avoid obstacles and reach the goal in a 3D space. However, in most wheel robot applications, a robot is driving on a 2D plane and a 2D map is sufficient to achieve navigation task. For those project/robot, laser scanners based mapping methods such as Gmapping can be used and using an RGB camera like Kinect for mapping, camera imagery, depth perception and etc,.. give an accurate result since, RGBD sensors are low FoV and short-range sensors which gives an accurate result with RGBD mapping and Rtab-map (3D). Realtime Appearance-Based Mapping(RTAB-Map) is an RGB-D Graph-Based SLAM approach based on an incremental appearance-based loop closure detector.

### Robot Model
The robot base model design and developed with the inspirations from Roomba home vacuum cleaning robot. The robot model is base is round with 2 wheels and to maintain the balance the two caster wheels under hold. Robot model equipped with a RGB\-D Kinect camera and a hokuyo laser sensor for distance, depth. To avoid the data miss measurements and detection errors, the Kinect sensor sticked front side of the robot and laser scanner which is place just in the top middle center, little above (z axes) to kinect to get the accurate results. All the necessary URDF and Gazebo files are in the below github code link.

## ** Deleted Source and Solution files as per Udacity Terms
