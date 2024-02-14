# Use the Docker Development Environment
After cloning this repository, source `bash_utils`.
```bash
. appld_simulation_environment/Docker/bash_utils
rosd-dir appld_simulation_environment/
```

Build the Docker image.
```bash
rosd-build
```

Run the container and open a shell inside it
```bash
rosd-start
rosd-shell
```
## Launch Gazebo Simulation
Inside the Docker container, build the workspace.
```bash
cd appld_ws/
catkin_make
```
Launch Gazebo.
```bash
. devel/setup.bash
roslaunch warthog_gazebo appld_gazebo_demo.launch
```