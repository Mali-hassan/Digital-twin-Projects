# 🤖 Multibot Navigation using ROS2, Gazebo, and Nav2

This project demonstrates **multi-robot autonomous navigation** in a simulated environment using **ROS2**, **Gazebo**, and **Nav2 (Navigation2 stack)**.  
It’s part of the **Digital Twin Projects** series, focusing on *multi-robot coordination, mapping,* and *autonomous navigation* in realistic simulation environments.  
Each robot runs an independent navigation stack and communicates through separate namespaces to avoid topic and TF conflicts.

---

## ✨ Key Features

- 🧩 Multi-robot setup in Gazebo world  
- 🚀 Independent namespaces for each robot (`/tb3_0`, `/tb3_1`, etc.)  
- 🗺️ SLAM and map sharing capabilities  
- 🤖 Path planning and collision avoidance using Nav2  
- ⚙️ Launch-based configuration for scalable multi-robot deployment  

---

## 🧰 Tech Stack

| Component | Description |
|------------|-------------|
| **ROS2 (Humble)** | Robotics middleware for communication and control |
| **Gazebo** | 3D simulation environment for physics and visuals |
| **Nav2** | Navigation stack for path planning, control, and obstacle avoidance |
| **RViz2** | Visualization tool for debugging and monitoring |
| **TurtleBot3** | Differential drive mobile robot model |

---

## ⚙️ How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/<your-username>/Digital-twin-Projects.git
cd Digital-twin-Projects/Multibot-Navigation
````

### 2. Source ROS2 and Build Workspace

```bash
source /opt/ros/humble/setup.bash
colcon build
source install/setup.bash
```

### 3. Launch the Multi-Robot Simulation

```bash
ros2 launch multibot_nav multibot_world.launch.py
```

This will:

* Spawn multiple TurtleBots in Gazebo
* Launch individual Nav2 stacks
* Open RViz for real-time visualization

---

## 🌐 Digital Twin Integration

This simulation acts as a **digital twin** for real-world autonomous systems.
Each virtual TurtleBot3 mirrors the motion, control logic, and sensor data of a physical robot — allowing for **safe testing**, **rapid iteration**, and **real-time comparison** between simulation and hardware.

**Highlights:**

* **Real-World Mapping:** Gazebo environments replicate lab layouts for direct SLAM data transfer.
* **ROS2 Parity:** Identical topics, parameters, and TF trees between sim and physical robots.
* **Nav2 Consistency:** Same navigation stack ensures predictable real-world deployment.
* **Scalable Twins:** Namespace isolation (`/tb3_0`, `/tb3_1`, etc.) enables multi-robot digital twins for fleet coordination and mission planning.

---

## 🚀 Future Enhancements

* 🧠 Implement consensus algorithms for swarm decision-making
* 🦾 Integrate reinforcement learning (RL) for adaptive navigation
* 🪩 Add real-time digital twin visualization synced with physical robots

---

## 👨‍💻 Author

**Muhammad Ali Hassan**
B.E. Electrical Engineering, NUST
📧 *[malihassan0330@gmail.com]*
📍 Islamabad, Pakistan




