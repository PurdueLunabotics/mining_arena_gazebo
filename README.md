# mining_arena_gazebo
Gazebo world environments for the NASA competition
## What's in here?
Lunabotics 2021-2022 competition arena assets and world files

## Models
- Apriltag assets
- arena assets with correct dimensions
## Worlds
- arena.world: Full arena with apriltags

## Setup
1. Clone repo into purdue_lunabotics repo
2. Add models to ~/.bashrc to allow gazebo to find the model files
```
export GAZEBO_MODEL_PATH=/home/https://github.com/koide3/gazebo_apriltaguser/catkin_ws/src/purdue_lunabotics/lunabot_gazebo/models
```
3. Run with `gazebo arena.world` to visualize (ensure gazebo is installed)

## Credits
Apriltag assets from https://github.com/koide3/gazebo_apriltag
