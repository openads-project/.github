# OpenADS - Open Automated Driving Systems

> 🚧 Warning: This project is currently under construction.

![OpenADS diagram](../assets/openads-lab-diagram.svg)

## Documentation

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openads-project.github.io](https://github.com/openads-project/openads-project.github.io) | [**Documentation of the OpenADS ecosystem**](https://openads-project.github.io), including automated driving software stack, simulation and development toolchain. | 🚧 Under Construction |
| [tutorial-itsc-26](https://github.com/openads-project/tutorial-itsc-26) | [Website](https://openads-project.github.io/tutorial-itsc-26/) for OpenADS tutorial on IEEE ITSC 2026 in Naples, Italy. | ✅ Active |

## OpenADStack - The Automated Driving Stack

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openadstack](https://github.com/openads-project/openadstack) | Full AD stack compositions for different use cases | 🚧 Under Construction |

### Perception

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [point_cloud_fusion]() | GPU-accelerated (early) fusion of point clouds from multiple (lidar) sensors. | 📋 Planned |
| [point_cloud_object_detection]() | ML-based 3D object detection in lidar point clouds, which is trained, e.g., on the DrivIng dataset | 📋 Planned |
| [point_cloud_object_clustring]() | clusters object points (e.g. vehicles/pedestrians) for visualization in HMI | 📋 Planned |
| [autoware_ground_segmentation_cuda]() | GPU-accelerated whitebox (non-AI) ground filter for lidar point clouds, could be part of a (non-AI) safety layer | 📋 Planned |
| []() |  | 📋 Planned |
| [traffic_light_detection]() | Detect location and state of traffic lights using YOLOv5. | 📋 Planned |

### Understanding

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| []() |  | 🚧 Under Construction |

### Planning

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [lanelet2_map_server](https://github.com/openads-project/lanelet2_map_server) | ROS 2 HD Map Server for Automated Driving based on Lanelet2 | 🚧 Under Construction |
| [lanelet2_route_planning](https://github.com/openads-project/lanelet2_route_planning) | ROS 2 Route Planning for Automated Driving based on Lanelet2 | 🚧 Under Construction |
| [trajectory_optimization](https://github.com/openads-project/trajectory_optimization) | ROS 2 Trajectory Optimization for Automated Driving based on an Optimal Control Problem (OCP). | ✅ Active |
| [ackermann_trajectory_control](https://github.com/openads-project/ackermann_trajectory_control) | Cascaded ROS 2 PID Controller for Ackermann steered vehicles | 🚧 Under Construction |

## OpenADSim - The Simulation Environment

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openadsim]() |  | 🚧 Under Construction |
| [carla-simulator]() |  | 🚧 Under Construction |
| [carla-ros-bridge]() |  | 🚧 Under Construction |
| [carla-scenario-runner]() |  | 🚧 Under Construction |
| [carla_scenario_runner_ros]() |  | 🚧 Under Construction |
| [middleware-bridge]() |  | 🚧 Under Construction |
| [carla_converter]() |  | 🚧 Under Construction |
| [sumo_converter]() |  | 🚧 Under Construction |
| [simulation_adapter]() |  | 🚧 Under Construction |

## OpenADSuite - The Development Suite

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openads-dev-environment](https://github.com/openads-project/openads-dev-environment) | Common development environment for OpenADS modules | ✅ Active |
| [openads_demo_module](https://github.com/openads-project/openads_demo_module) | OpenADS ROS 2 Demo Repository | ✅ Active |

## Contribution

We are currently in the community building process and will establish a governance model and working groups to coordinate collaboration in this project. Meanwhile, we welcome contributions via issues or pull requests in the repositories.
