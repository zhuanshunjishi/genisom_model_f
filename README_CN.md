# 智身机器人 URDF 模型

[English version](./README.md) · [BSD 3-Clause 许可证](./LICENSE)

本仓库提供五款智身四足机器人的 URDF 模型和 STL 网格。每个 URDF 描述对应机器人的连杆、关节、惯性参数和几何形状。

## 型号与文件

| 机器人型号 | URDF 文件 | STL 网格 |
| --- | --- | --- |
| Genisom L1 | [ZSL-1.urdf](Genisom%20L1/urdf/ZSL-1.urdf) | [meshes/](Genisom%20L1/meshes/) |
| Genisom L1 EDU | [DOG.urdf](Genisom%20L1%20EDU/urdf/DOG.urdf) | [meshes/](Genisom%20L1%20EDU/meshes/) |
| Genisom L1-W | [ZSL-1W.urdf](Genisom%20L1-W/urdf/ZSL-1W.urdf) | [meshes/](Genisom%20L1-W/meshes/) |
| Genisom L1-W EDU | [xg_wheel_su.urdf](Genisom%20L1-W%20EDU/urdf/xg_wheel_su.urdf) | [meshes/](Genisom%20L1-W%20EDU/meshes/) |
| Genisom M1 | [ZG_M1_A0_V1_0.urdf](Genisom%20M1/urdf/ZG_M1_A0_V1_0.urdf) | [meshes/](Genisom%20M1/meshes/) |

## 加载模型

下载所需型号的完整目录，保持 `urdf/` 和 `meshes/` 为同级目录。使用支持按 URDF 文件位置解析相对路径的查看器，打开表中对应的 URDF。例如，L1 的 `Genisom L1/urdf/ZSL-1.urdf` 通过 `../meshes/BASE_LINK.STL` 加载机身网格。

**L1 EDU 驱动仿真。** L1 EDU 的 12 个活动关节在 URDF 中均设为 `effort="0"` 和 `velocity="0"`。如需驱动仿真，请先按 L1 EDU 的硬件规格核实力矩和速度上限，再配置控制器。
