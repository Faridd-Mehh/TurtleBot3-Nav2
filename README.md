
# TurtleBot3 Navigation with RViz and Map

This project demonstrates how to control a TurtleBot3 robot in a Gazebo environment using RViz and a pre-built map. The robot is controlled by sending navigation goals through RViz, and the robot navigates towards the target using the provided map.

## How to Run

 Launch the Gazebo Environment:
First, start the Gazebo simulation for TurtleBot3 using the following command:

```bash
ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py

This will open the Gazebo simulation with the TurtleBot3 model in the environment.

Once Gazebo is running, you need to launch the navigation stack. This includes the map server and navigation2 nodes:

ros2 launch turtlebot3_navigation2 navigation2_launch.py map:=/path/to/your/map.yaml
Replace /path/to/your/map.yaml with the correct path to your map file.

After open RViz to visualize the robot and interact with it. In RViz, you can set goals for the robot to navigate to.
