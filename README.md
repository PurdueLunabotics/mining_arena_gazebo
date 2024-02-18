# mining_arena_gazebo
Gazebo world environments for the NASA competition
## What's in here?
Lunabotics 2023-2024 competition arena assets and world files

## Models
- Apriltag assets
- arena assets with correct dimensions
## Worlds
- arena_nasa.world: Kennedy space center Arena (2024 competition)
- arena_ucf.world: UCF Arena (2024 competition)

## Setup
1. Ensure that repo is placed at `purdue_lunabotics/lunabot_sim/<here>`
2. Add models and plugins to ~/.bashrc to allow gazebo to find the model/plugin files
```
export GAZEBO_MODEL_PATH=~/catkin_ws/src/purdue_lunabotics/lunabot_sim/mining_arena_gazebo/models:$GAZEBO_MODEL_PATH
export GAZEBO_PLUGIN_PATH=~/catkin_ws/devel/lib:$GAZEBO_PLUGIN_PATH

```
3. Run with `gazebo arena.world` to visualize (ensure gazebo is installed)

## Running sim: 
Launch sim:
```
roslaunch lunabot_bringup sim.launch
```

Options:
`KSC_arena:=<true/false>`
(Use KSC or UCF arena)

Remove repeated warnings: append `2> >(grep -v TF_REPEATED_DATA buffer_core)` to the end of the command.

(This won't print any lines with the words `TF_REPEATED_DATA` or `buffer_core`)

![sim_nav_gazebo](https://user-images.githubusercontent.com/41026849/163585429-cf9080de-40e7-4be1-9648-d75ab31ae4af.png)

## Credits
Apriltag assets from https://github.com/koide3/gazebo_apriltag
