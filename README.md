# pixi_rox — Reproducible Neobotix ROX ROS 2 Jazzy Workspace with Pixi

This repository defines a fully reproducible **ROS 2 Jazzy** development and simulation environment using [Pixi](https://pixi.sh/dev/tutorials/ros2/).  
All dependencies, packages, and build steps are automated so that anyone can recreate the same workspace on any machine.



---

### 🚀 Reproduce this workspace anywhere

Clone the repository and enter the project directory:

```bash
https://github.com/AshinTheAnvil/pixi_rox.git
cd pixi_rox
```

Then follow these steps to set up and run everything:

```bash
# 1️⃣ Create identical ROS Jazzy environment()
pixi install

# 2️⃣ Fetch all NeoBotix source packages into src/
pixi run fetch_neobotix_pkgs

# 3️⃣ Build the workspace with colcon
pixi run colcon build --symlink-install

# 4️⃣ Launch the simulation / bring‑up
pixi run ros2 launch rox_bringup bringup_sim_launch.py
```

After these commands, your system will have a fully built and runnable ROS 2 Jazzy workspace with Neobotix ROX pkgs managed by Pixi.
