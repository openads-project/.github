# OpenADS - Open Automated Driving Systems

<p align="center">
  <a href="https://github.com/openads-project"><img src="https://img.shields.io/badge/OpenADS-f5ff01"/></a>
  <a href="https://www.ros.org"><img src="https://img.shields.io/badge/ROS 2-jazzy-22314e"/></a>
  <a href="https://openads-project.github.io"><img src="https://img.shields.io/badge/Documentation-OpenADS-brightgreen"/></a>
</p>

> 🚧 Warning: This project is currently under construction.

| Main Repository | Release | Documentation |
| --------------- | ------- | ------------- |
| [OpenADStack](https://github.com/openads-project/openadstack) 🚧 | [![](https://img.shields.io/github/v/release/openads-project/openadstack)](https://github.com/openads-project/openadstack/releases/latest) | [![](https://img.shields.io/badge/Documentation-OpenADStack-brightgreen)](https://openads-project.github.io/openadstack) |
| [OpenADSim](https://github.com/openads-project/openadsim) 🚧 | [![](https://img.shields.io/github/v/release/openads-project/openadsim)](https://github.com/openads-project/openadsim/releases/latest) | [![](https://img.shields.io/badge/Documentation-OpenADSim-brightgreen)](https://openads-project.github.io/openadsim) |

### Collaborative development and benchmark-driven evaluation

OpenADS explores how distributed partners can build compatible automated driving services and use benchmarks to identify stronger system compositions. The work is embedded in Germany's [Ecosystem Mobility 4.0](https://ecosystemmobility40.de/en/home/) initiative and aligned with the goals of the [European Connected and Autonomous Vehicle Alliance](https://digital-strategy.ec.europa.eu/en/policies/vehicle-alliance).

![OpenADS diagram](../assets/openads-diagram.svg)

## Repositories

> Repositories tagged with 🔗 are not hosted in the [openads-project](github.com/openads-project/) GitHub organization.

### Documentation

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openads-project.github.io](https://github.com/openads-project/openads-project.github.io) | [**Documentation of the OpenADS ecosystem**](https://openads-project.github.io), including automated driving software stack, simulation and development toolchain. | 🚧 Under Construction |
| [tutorial-itsc-26](https://github.com/openads-project/tutorial-itsc-26) | [Website](https://openads-project.github.io/tutorial-itsc-26/) for OpenADS tutorial on IEEE ITSC 2026 in Naples, Italy. | ✅ Active |

### OpenADSuite - The Development Suite

#### Development

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openads_demo_module](https://github.com/openads-project/openads_demo_module) | Template for new OpenADS modules including OpenADSuite development environment and CI/CD workflows | ✅ Active |
| [ros2-pkg-create](https://github.com/ika-rwth-aachen/ros2-pkg-create) 🔗 | Powerful ROS 2 Package Generator. | ✅ Active |
| [openads-dev-environment](https://github.com/openads-project/openads-dev-environment) | Common development environment for OpenADS modules | ✅ Active |
| [docker-ros](https://github.com/ika-rwth-aachen/docker-ros) 🔗 | docker-ros automatically builds development and deployment Docker images for your ROS-based repositories. | ✅ Active |
| [docker-ros-ml-images](https://github.com/ika-rwth-aachen/docker-ros-ml-images) 🔗 | Machine Learning-Enabled ROS Docker Images. | ✅ Active |
| [docker-run](https://github.com/ika-rwth-aachen/docker-run) 🔗 | CLI tool for simplified interaction with Docker images. | ✅ Active |

#### Monitoring

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [monitoring](https://github.com/openads-project/monitoring) | Monitoring and visualization using [RViz](https://github.com/ros2/rviz) with support for message definitions used in OpenADS. | ✅ Active |
| [lichtblick]() | Web-based visualization using [Lichtblick](https://github.com/lichtblick-suite/lichtblick) with support for message definitions used in OpenADS. | 📋 Release Planned |

#### Interfaces

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [perception_interfaces](https://github.com/ika-rwth-aachen/perception_interfaces) 🔗 | ROS packages with common messages and tools relating to the perception task in automated driving and C-ITS. | ✅ Active |
| [planning_interfaces](https://github.com/ika-rwth-aachen/planning_interfaces) 🔗 | ROS packages with common messages and tools relating to the behavior planning task of automated vehicles. | ✅ Active |
| [etsi_its_messages](https://github.com/ika-rwth-aachen/etsi_its_messages) 🔗 | ROS 2 Support for ETSI ITS Messages for V2X Communication. | ✅ Active |
| [omega-prime](https://github.com/ika-rwth-aachen/omega-prime) 🔗 | Data Model, Data Format and Python Library for Handling Ground Truth Traffic Data. | ✅ Active |

### OpenADStack - The Automated Driving Stack

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openadstack](https://github.com/openads-project/openadstack) | Full stack compositions for different automated driving use cases | 🚧 Under Construction |

### OpenADServices - Modular Functional Building Blocks for Full-Stack Compositions

#### Perception

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [point_cloud_fusion](https://github.com/openads-project/point_cloud_fusion) | GPU-accelerated (early) fusion of point clouds from multiple (lidar) sensors. | ✅ Active |
| [point_cloud_object_detection]() | ML-based 3D object detection in lidar point clouds, which is trained, e.g., on the DrivIng dataset. | 📋 Release Planned |
| [point_cloud_object_clustring]() | clusters object points (e.g. vehicles/pedestrians) for visualization in HMI. | 📋 Release Planned |
| [autoware_ground_segmentation_cuda]() | GPU-accelerated whitebox (non-AI) ground filter for lidar point clouds, could be part of a (non-AI) safety layer. | 📋 Release Planned |
| [autoware_probabilistic_occupancy_grid_map]() | GPU-accelerated whitebox (non-AI) occupancy grid mapping from lidar point clouds, could be part of a (non-AI) safety layer. | 📋 Release Planned |
| [traffic_light_detection]() | Detector for location and state of traffic lights using YOLOv5. | 📋 Release Planned |

#### Understanding

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [simple_object_tracking]() | (Late) fusion of 3D object lists. | 📋 Release Planned |
| [lanelet2_object_list_prediction]() | Dynamic object prediction based on Lanelet2 map information and kinematic models. | 📋 Release Planned |
| [dynamic_map_enrichment]() | Enriches route information with regulatory elements (e.g. traffic light states). | 📋 Release Planned |

#### Planning

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [ego_state_estimation]() | Dynamics state estimation for ego vehicle based on GNSS and IMU data. | 📋 Release Planned |
| [lanelet2_map_server](https://github.com/openads-project/lanelet2_map_server) | ROS 2 HD Map Server for Automated Driving based on Lanelet2. | ✅ Active |
| [lanelet2_route_planning](https://github.com/openads-project/lanelet2_route_planning) | ROS 2 Route Planning for Automated Driving based on Lanelet2. | ✅ Active |
| [simple_planner]() | Plans a reference trajectory based on route and Lanelet2 map. | 🚧 Under Construction |
| [planning_orchestrator]() | Switches between different planning modules, e.g. rule-based vs. AI planner. | 📋 Release Planned |
| [trajectory_optimization](https://github.com/openads-project/trajectory_optimization) | ROS 2 Trajectory Optimization for Automated Driving based on an Optimal Control Problem (OCP). | ✅ Active |
| [ackermann_trajectory_control](https://github.com/openads-project/ackermann_trajectory_control) | Cascaded ROS 2 PID Controller for Ackermann steered vehicles. | ✅ Active |

### OpenADSim - The Simulation Environment

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [openadsim]() | Simulation environment for running and testing OpenADStack with CARLA or SUMO. | 🚧 Under Construction |
| [carla-simulator](https://github.com/openads-project/carla-simulator) | High-fidelity rendering and physics backend based on CARLA for closed-loop sensor and vehicle simulation. | ✅ Active |
| [carla-ros-bridge](https://github.com/openads-project/carla-ros-bridge) | ROS 2 connection to CARLA topics, services, exposing simulator state and controls to the OpenADS ecosystem. | ✅ Active |
| [carla-scenario-runner](https://github.com/openads-project/carla-scenario-runner) | Execution of OpenSCENARIO scenarios in CARLA for repeatable scenario-based simulation and testing. | ✅ Active |
| [ros_middleware_bridge](https://github.com/openads-project/ros_middleware_bridge) | DDS-to-Zenoh bridge that connects CARLA native ROS communication with the OpenADStack middleware. | ✅ Active |
| [carla_converter](https://github.com/openads-project/carla_converter) | Conversion of CARLA-specific simulation outputs into OpenADS-compatible ego, object, map, and V2X topics. | ✅ Active |
| [sumo_converter]() | Conversion of SUMO traffic simulation data into OpenADS-compatible ego, object, and map topics. | 🚧 Under Construction |
| [simulation_adapter](https://github.com/openads-project/simulation_adapter) | Backend-independent adapter that normalizes simulator outputs and connects OpenADStack. | ✅ Active |

### OpenADSafety - The Verification & Validation Framework

| Repository | Description | Status |
| ---------- | ----------- | ------ |
| [autonomy_datasets](https://github.com/thinking-cars/autonomy_datasets) 🔗 | Unified ROS 2 Interface for automated driving datasets. | ✅ Active |
| [autonomy_benchmarks](https://github.com/thinking-cars/autonomy_benchmarks) 🔗 | Transparent benchmarks for automated driving building blocks and full stacks across different tasks and datasets. | 🚧 Under Construction |

## Contribution

We are currently in the community building process and will establish a governance model and working groups to coordinate collaboration in this project. Meanwhile, we welcome contributions via issues or pull requests in the repositories.
