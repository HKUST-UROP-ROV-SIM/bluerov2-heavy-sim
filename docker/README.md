# Attention
In [run.sh](run.sh), please uncomment the code block according to your computer graphics card's driver.

# Bulding the docker image
1. To build the docker image:
```
./build.sh
```
# Running the docker image
1. At the first time, please mount the screen to the image:
```
xhost +local:root
```
2. To launch Gazebo, RViz, all nodes:
```
./run.sh
ros2 launch orca_bringup sim_launch.py
```
3. To execute a mission:
```
docker exec -it orca4 /bin/bash
ros2 run orca_bringup mission_runner.py
```
