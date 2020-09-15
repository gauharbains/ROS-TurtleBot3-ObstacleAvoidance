# ROS-TurtleBot3-ObstacleAvoidance


This submission consists of the `ObstacleAvoidance` ROS package. 

## Compile and run Package
```
1. Please paste this package in the 'src' directory of your catkin workspace and run `catkin_make`
2. Run `rospack profile`
3. Launch the gazebo environment at (x,y)= (-2,0) (or any desired postion) using --> roslaunch turtlebot3_gazebo turtlebot3_world.launch x_pos:=-2 y_pos:=0
4. Run the turtlebot_controller.py node from the package `ObstacleAvoidance` using ----> rosrun ObstacleAvoidance turtlebot3_controller.py 
5. The program exits after all goals have been reached.
```

## Task 


The following tasks should be accomplished by the robot. Changes can be made to the starting point and list of waypoints in line 129 of `turtlebot_controller.py`.
At present, line 129 specifies the following waypoints based on the goal description below : `waypoints = [(1,-2), (-1,2),(2,0), (-1,-2), (1,2)]`

####  1. Reach Goals
```
1. Spawn the TurtleBot3 at position (-2,0) as shown in Figure below.
2. From the start position (-2,0), drive the TurtleBot in a straight line to the following goals:
    * Pillar 1 (1,-2), then
    * Pillar 1 (-1,2), then
    * Pillar 1 (2,0), then
    * Pillar 1 (-1,-2), then
    * Pillar 1 (1,2), then  
 ```
            


#### 2. Obstacle Avoidance 
Obstacle avoidance has been implemented to enable the turtlebot to reach the goals. Data from the LaserScan (LIDAR sensors) on the TurtleBot3 has been used to develop an obstacle avoidance algorithm. 


<img align="center" width="487" alt="maze" src="https://user-images.githubusercontent.com/48079888/93158755-cd8b8e00-f6da-11ea-907a-d6f5a62e3261.PNG">

