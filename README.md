# GENISOM-AI URDF Models

[中文版本](./README_CN.md) · [BSD 3-Clause License](./LICENSE)

This repository contains URDF descriptions and STL meshes for five GENISOM-AI quadruped models. Each URDF defines the robot’s links, joints, inertial properties, and geometry.

## Models

| Robot | URDF file | STL meshes |
| --- | --- | --- |
| Genisom L1 | [ZSL-1.urdf](Genisom%20L1/urdf/ZSL-1.urdf) | [meshes/](Genisom%20L1/meshes/) |
| Genisom L1 EDU | [DOG.urdf](Genisom%20L1%20EDU/urdf/DOG.urdf) | [meshes/](Genisom%20L1%20EDU/meshes/) |
| Genisom L1-W | [ZSL-1W.urdf](Genisom%20L1-W/urdf/ZSL-1W.urdf) | [meshes/](Genisom%20L1-W/meshes/) |
| Genisom L1-W EDU | [xg_wheel_su.urdf](Genisom%20L1-W%20EDU/urdf/xg_wheel_su.urdf) | [meshes/](Genisom%20L1-W%20EDU/meshes/) |
| Genisom M1 | [ZG_M1_A0_V1_0.urdf](Genisom%20M1/urdf/ZG_M1_A0_V1_0.urdf) | [meshes/](Genisom%20M1/meshes/) |

## Loading a model

Download the complete model directory and keep its `urdf/` and `meshes/` folders side by side. Open the URDF listed above in a viewer that resolves mesh paths relative to the URDF file. For example, the L1 model loads `../meshes/BASE_LINK.STL` from `Genisom L1/urdf/ZSL-1.urdf`.

**L1 EDU simulation.** All 12 actuated joints in the L1 EDU URDF have `effort="0"` and `velocity="0"`. For actuated simulation, verify the torque and velocity limits against the L1 EDU hardware specifications before configuring the controller.
