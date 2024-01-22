# Maze maps

## Use
Place the maze map (.world) in the following directory:
```
/home/carl/turtlebot3_ws/src/turtlebot3_simulations/turtlebot3_gazebo/worlds
```
Create a symbolic link to this file from the following directory:
```
/home/carl/turtlebot3_ws/install/turtlebot3_gazebo/share/turtlebot3_gazebo/worlds
```
using:
```
ln -s /home/carl/turtlebot3_ws/src/turtlebot3_simulations/turtlebot3_gazebo/worlds/maze.world
```

Create a new launch py file in the following directory by copying one of the existing ones in it:
```
/home/carl/turtlebot3_ws/src/turtlebot3_simulations/turtlebot3_gazebo/launch
```
e.g:
```
cp empty_world.launch.py maze.launch.py
```
Edit the following line in the new file (the copy), exchanging the empty_world.world to the desired maze map:
```
world = os.path.join(
        get_package_share_directory('turtlebot3_gazebo'),
        'worlds',
        'empty_world.world'
    )
```
Create a symbolic link to this new launch file from the following directory:
```
/home/carl/turtlebot3_ws/install/turtlebot3_gazebo/share/turtlebot3_gazebo/launch
```
using:
```
ln -s /home/carl/turtlebot3_ws/src/turtlebot3_simulations/turtlebot3_gazebo/launch/maze.launch.py
```

## Disclaimer
The exact paths need to be altered for the target system.

## License
Distributed under the MIT license.


## Contact
Carl Larsson - cln20001@student.mdu.se
