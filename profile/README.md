<p align="center">
  <a href="https://openads-project.github.io">
    <img src="https://raw.githubusercontent.com/openads-project/openads-project.github.io/refs/heads/main/docs/assets/openads-logo.svg" alt="OpenADS – Open Automated Driving: Stack, Sim, Suite, Safety" width="340">
  </a>
</p>

# OpenADS – Open Automated Driving Systems

**OpenADS is an open-source ecosystem for connected and autonomous driving built on [ROS 2](https://www.ros.org/).** It provides a complete reference software stack for SAE Level 4 automated driving, simulation with [CARLA](https://carla.org/) and [SUMO](https://eclipse.dev/sumo/), developer tools, and benchmarks for verification and validation – released under the Apache 2.0 license. OpenADS runs on real research vehicles and road infrastructure. It is open to partners from research and industry (see [🤝 Support](https://openads-project.github.io/support/support.html)).

**[📖 Documentation](https://openads-project.github.io)** · **[🚀 Quick Start](https://openads-project.github.io/start/start.html)** · **[🎬 Video](https://www.youtube.com/watch?v=B0Lnu-1w9KE)** · **[📋 Backlog](https://github.com/orgs/openads-project/projects/5)** · **[🤝 Support](https://openads-project.github.io/support/support.html)**

## The OpenADS Ecosystem

![OpenADS ecosystem diagram: OpenADServices (perception, planning, control), OpenADStack (full reference automated driving stack), OpenADSim (scenario-based testing), OpenADSuite (development tools) and OpenADSafety (verification and validation, benchmarks)](https://raw.githubusercontent.com/openads-project/openads-project.github.io/refs/heads/main/docs/assets/openads-diagram.svg)

| Component | Description | Release | Documentation |
| --------- | ----------- | ------- | ------------- |
| 🤖 [**OpenADStack**](https://github.com/openads-project/openadstack) | Open-source Level 4 automated driving stack on ROS 2: localization, perception, prediction, planning and control in a Docker Compose based reference stack. | [![OpenADStack release](https://img.shields.io/github/v/release/openads-project/openadstack)](https://github.com/openads-project/openadstack/releases/latest) | [OpenADStack](https://openads-project.github.io/openadstack/openadstack.html) |
| 🧩 [**OpenADServices**](https://github.com/search?q=topic%3Aopenadservice+org%3Aopenads-project&type=repositories) | Modular, reusable ROS 2 building blocks that make up the stack and can also be used on their own. | multiple | [Functional architecture](https://openads-project.github.io/openadstack/openadstack/docs/functional-architecture.html) |
| 🎮 [**OpenADSim**](https://github.com/openads-project/openadsim) | Closed-loop simulation and scenario-based testing of the stack with CARLA or SUMO. | [![OpenADSim release](https://img.shields.io/github/v/release/openads-project/openadsim)](https://github.com/openads-project/openadsim/releases/latest) | [OpenADSim](https://openads-project.github.io/openadsim/openadsim.html) |
| 🛠️ [**OpenADSuite**](https://github.com/search?q=topic%3Aopenadsuite+org%3Aopenads-project&type=repositories) | Developer tools: module template, development environment, Helm charts, monitoring and ROS 2 analysis tools. | multiple | [OpenADSuite](https://openads-project.github.io/openadsuite/openadsuite.html) |
| 🛡️ [**OpenADSafety**](https://github.com/search?q=topic%3Aopenadsafety+org%3Aopenads-project&type=repositories) 🚧 | Tools and transparent benchmarks for verification and validation of automated driving modules and full stacks. | in progress | [OpenADSafety](https://openads-project.github.io/openadsafety/openadsafety.html) |

## Quick Start

Try OpenADStack in a few minutes: the demo runs the stack open-loop on recorded ROS 2 data (Docker required).

```bash
git clone https://github.com/openads-project/openadstack.git
cd openadstack/demo
xhost +local:
docker compose up -d
```

For closed-loop simulation with CARLA or SUMO, start with [OpenADSim](https://github.com/openads-project/openadsim). System requirements and further options are described in the [Quick Start guide](https://openads-project.github.io/start/start.html).

## Modules by Domain

| Domain | Repositories |
| ------ | ------------ |
| Localization & maps | [lanelet2_map_server](https://github.com/openads-project/lanelet2_map_server) – ROS 2 HD Map Server for Automated Driving based on Lanelet2 |
| Perception | [point_cloud_object_detection](https://github.com/openads-project/point_cloud_object_detection) – ROS 2 Point Cloud Object Detection for Automated Driving<br>[point_cloud_fusion](https://github.com/openads-project/point_cloud_fusion) – ROS 2 Point Cloud Fusion of Multiple Point Clouds into a Single Point Cloud<br>[pcod-common](https://github.com/openads-project/pcod-common) – Shared Preprocessing and Postprocessing Library for Point Cloud Object Detection<br>[triton_cpp](https://github.com/openads-project/triton_cpp) – Wrapper for Triton C++ Client Libraries |
| Prediction | [lanelet2_object_list_prediction](https://github.com/openads-project/lanelet2_object_list_prediction) – ROS 2 Object List Prediction for Automated Driving based on Lanelet2 |
| Planning | [lanelet2_route_planning](https://github.com/openads-project/lanelet2_route_planning) – ROS 2 Route Planning for Automated Driving based on Lanelet2<br>[simple_planner](https://github.com/openads-project/simple_planner) – ROS 2 Reference Trajectory Planning for Automated Driving<br>[trajectory_optimization](https://github.com/openads-project/trajectory_optimization) – ROS 2 Trajectory Optimization for Automated Driving based on an Optimal Control Problem (OCP) |
| Control | [ackermann_trajectory_control](https://github.com/openads-project/ackermann_trajectory_control) – Cascaded ROS 2 PID Controller for Ackermann steered vehicles |
| Simulation & bridges | [carla-simulator](https://github.com/openads-project/carla-simulator) – High-fidelity rendering and physics backend based on CARLA for closed-loop sensor and vehicle simulation<br>[carla-ros-bridge](https://github.com/openads-project/carla-ros-bridge) – Bidirectional communication bridge between CARLA simulation and ROS ecosystems<br>[carla-scenario-runner](https://github.com/openads-project/carla-scenario-runner) – OpenSCENARIO execution for scenario-based testing and evaluation in CARLA<br>[carla_converter](https://github.com/openads-project/carla_converter) – Converter for CARLA specific ROS 2 data to OpenADS interfaces<br>[simulation_adapter](https://github.com/openads-project/simulation_adapter) – Adapts OpenADSim data to vehicle-specific OpenADStack interfaces<br>[ros_middleware_bridge](https://github.com/openads-project/ros_middleware_bridge) – ROS 2 middleware bridge serializing topic data between different RMW implementations |
| Developer tools | [openads-dev-environment](https://github.com/openads-project/openads-dev-environment) – Common development environment for OpenADS modules<br>[openads_demo_service](https://github.com/openads-project/openads_demo_service) – Template repository for new OpenADServices<br>[openads-helm](https://github.com/openads-project/openads-helm) – Essential OpenADS Helm Charts<br>[monitoring](https://github.com/openads-project/monitoring) – Monitoring and visualization using RViz and RQt with support for message definitions used in OpenADS<br>[ros2_graph_export](https://github.com/openads-project/ros2_graph_export) – ROS 2 Node and Topic Graph Exporter<br>[ros2_unbag_plugins](https://github.com/openads-project/ros2_unbag_plugins) – Plugins for ros2_unbag topic export with the openADS interfaces<br>[ros2-trace-analysis](https://github.com/openads-project/ros2-trace-analysis) – Analyze ROS 2 execution traces to understand system performance and timing behavior<br>[openads-assets](https://github.com/openads-project/openads-assets) – Shared 3D meshes and URDF robot descriptions for OpenADS |

## Where OpenADS is used

<table>
  <tr>
    <td width="33%"><a href="https://karl.ac/"><img src="https://raw.githubusercontent.com/openads-project/openads-project.github.io/refs/heads/main/docs/assets/integration-karl.png" alt="karl. research vehicle for automated and connected driving"></a></td>
    <td width="33%"><a href="https://www.ika.rwth-aachen.de/en/competences/equipment/research-vehicles/unicaragil-autoshuttle-en.html"><img src="https://raw.githubusercontent.com/openads-project/openads-project.github.io/refs/heads/main/docs/assets/integration-autoshuttle.png" alt="autoSHUTTLE driverless research vehicle from the UNICARagil project"></a></td>
    <td width="33%"><a href="https://www.ika.rwth-aachen.de/en/competences/equipment/infrastructure/roadside-infrastructure.html"><img src="https://raw.githubusercontent.com/openads-project/openads-project.github.io/refs/heads/main/docs/assets/integration-rita.png" alt="RITA roadside infrastructure test field in Aachen"></a></td>
  </tr>
  <tr>
    <td><b>karl.</b> – ika's research vehicle for automated and connected driving</td>
    <td><b>autoSHUTTLE</b> – driverless shuttle built from scratch in UNICARagil</td>
    <td><b>RITA</b> – roadside infrastructure test field in Aachen</td>
  </tr>
</table>

Using OpenADS in your own vehicle, robot or test field? [Add your integration](https://github.com/openads-project/openads-project.github.io/edit/main/docs/index.md) to the documentation.

## Roadmap: A Hybrid Architecture for Safe Automated Driving

OpenADStack follows a *Doer/Checker/Fallback* pattern. The current release combines learned perception with a rule-based planner. Next, a learned planner will act as *Doer* while the rule-based planner remains the safety *Checker*, supported by an MLOps process for continual improvement (planned until the end of 2026). After that, an end-to-end driving model is planned as *Doer* (until the end of 2027). Details are in the [OpenADStack README](https://github.com/openads-project/openadstack#-architecture).

## Get Involved

OpenADS explores how distributed partners can build compatible automated driving services and use benchmarks to identify stronger system compositions. The work is embedded in Germany's [Ecosystem Mobility 4.0](https://ecosystemmobility40.de/en/home/) initiative and aligned with the goals of the [European Connected and Autonomous Vehicle Alliance (ECAVA)](https://digital-strategy.ec.europa.eu/en/policies/vehicle-alliance).

- See what we are working on in the [**backlog**](https://github.com/orgs/openads-project/projects/5).
- Ask questions, report bugs or propose features as described on the [**Support**](https://openads-project.github.io/support/support.html) page.
- Start a new module from the [**OpenADService template**](https://github.com/openads-project/openads_demo_service).
- Contact: [Public Matrix chat](https://matrix.to/#/#openads:matrix.org) or [opensource@ika.rwth-aachen.de](mailto:opensource@ika.rwth-aachen.de)

## Events

| Date | Place | Event |
| ---- | ----- | ----- |
| 15 September 2026 | Naples, Italy | [OpenADS Tutorial](https://openads-project.github.io/tutorial-itsc-26/) at the [IEEE International Conference on Intelligent Transportation Systems (ITSC)](https://ieee-itsc.org/2026/) – [slides](https://openads-project.github.io/tutorial-itsc-26/2026-09_15_ITSC_OpenADS.pdf) and [video](https://www.youtube.com/watch?v=xDkKu5G0FwI) available |

## Projects

OpenADS has been developed and used in national and European research projects, including [UNICARagil](https://www.unicaragil.de/en/), [autotech.agil](https://www.autotechagil.de/en/), [6GEM and 6GEM+](https://6gem.de/en/), [4CAD](https://www.ika.rwth-aachen.de/en/competences/projects/automated-driving/4-cad-en.html), [AIthena](https://aithena.eu/), [AIggregate](https://aiggregate.eu/), [SYNERGIES](https://synergies-ccam.eu/) and [iEXODUS](https://iexoddus-project.eu/).

---

<sub>OpenADS – Open Automated Driving Systems · open-source software for automated driving on ROS 2 · Apache 2.0</sub>
