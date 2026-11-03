# OpenHUTB

OpenHUTB 简单来说是面向人机共生与智能载具研究、教学和开发，提供影视级物理模拟器、开放数字资产，以及感知、规划、控制和场景生成工具的开源仿真社区。该社区具体提供一个包含人车代理（学术研究）、模拟器（技术开发包括数据驱动、机理仿真、界面渲染）、现实场景（艺术增强）的 [模拟器](https://openhutb.github.io) ，代理包括[感知](https://openhutb.github.io/doc/algorithms/perception/) （连接）、[规划](https://openhutb.github.io/doc/algorithms/planning/) （符号）、[控制](https://openhutb.github.io/doc/algorithms/control/) （行为）；模拟器包括 Python 与 C++ 的接口（正向创建、反向构建）、LibCarla、虚幻引擎插件；现实场景包括 [静态场景孪生](https://openhutb.github.io/doc/adv_digital_twin/) 、[动态场景孪生](https://github.com/OpenHUTB/traffic_twin/) 。


## 贡献想法与计划

社区文档连接开发环境、模型制作和项目协作。入门说明除了告诉读者点哪里、运行什么命令，还需要交代适用条件，以及完成后该检查什么。维护重点放在容易让操作中断或交付不完整的环节，保留已有示例，再补上缺失的步骤。

本轮围绕以下五个问题开展修改：

| 方向 | 具体改进 | 讨论与修改 |
| --- | --- | --- |
| Python 环境交接 | 保存版本和依赖清单，在新环境安装并检查，避免直接复制整个虚拟环境 | [问题 #453](https://github.com/OpenHUTB/.github/issues/453) · [修改 #458](https://github.com/OpenHUTB/.github/pull/458) |
| Blender 素材交付 | 检查缺失贴图，说明资源打包、相对路径和导出后的材质检查 | [问题 #454](https://github.com/OpenHUTB/.github/issues/454) · [修改 #459](https://github.com/OpenHUTB/.github/pull/459) |
| 虚拟机磁盘扩容 | 根分区被占用时从试用环境离线调整，再回到原系统核对容量 | [问题 #455](https://github.com/OpenHUTB/.github/issues/455) · [修改 #460](https://github.com/OpenHUTB/.github/pull/460) |
| Git 提交身份 | 区分作者信息与登录认证，补充仓库级配置和邮箱归属检查 | [问题 #456](https://github.com/OpenHUTB/.github/issues/456) · [修改 #461](https://github.com/OpenHUTB/.github/pull/461) |
| 提交统计工具 | 屏蔽名单格式有误时停止统计，保留原有结果，并覆盖异常输入测试 | [问题 #457](https://github.com/OpenHUTB/.github/issues/457) · [修改 #462](https://github.com/OpenHUTB/.github/pull/462) |

后续先跟进这五项修改的讨论，在各自分支处理反馈，核对最终差异和构建结果。文档中的命令、界面名称与适用范围一起检查；涉及分区或文件写入时，明确确认步骤和完成后的检查办法。脚本修改继续保留有效输入、异常输入和已有输出保护的测试，避免只验证正常情况。

参与审核时同时查看说明和完整差异，重点检查命令能否前后衔接、链接目标是否正确、示例与正文是否一致；发现问题时给出具体位置和可操作的建议。

## 社区入口

以下为新手快速上手栏目：

[🚀 快速开始](https://github.com/OpenHUTB/hutb#使用示例) · [📖 在线文档](https://openhutb.github.io/) · [🧪 运行示例](https://github.com/OpenHUTB/doc/tree/master/src/examples) · [🤝 参与贡献](https://github.com/OpenHUTB/.github/blob/master/CONTRIBUTING.md) · [💬 提问与讨论](https://github.com/orgs/OpenHUTB/discussions)
- [💡 贡献小贴士](contribute-tips.md)

你可以用 OpenHUTB 做什么？
- **研究与教学**：学习感知、规划、控制和具身智能算法。
- **仿真与验证**：在可重复的场景中开发、训练和验证算法。
- **场景与内容开发**：使用开放的城镇、建筑、车辆、行人和道具资产创建仿真环境。

核心入口

- 🟡 **[hutb 人车模拟器](https://github.com/OpenHUTB/hutb)** — 提供下载工具、Python API 和交通生成示例，目前持续开发中。
- 📚 **[doc 人车文档](https://github.com/OpenHUTB/doc)** — 人车模拟器配套安装说明、API与教程文档。

### 研究与实验项目

- 🧪 **[traffic_twin 人车孪生](https://github.com/OpenHUTB/traffic_twin)** — 交通数字孪生相关研究和示例，使用前请查看仓库说明。
- 🧠 **[neuro 神经原理](https://github.com/OpenHUTB/neuro)** — 用于感知与神经网络算法的相关研究与实验。
- 🧭 **[PFC 规划](https://github.com/OpenHUTB/PFC)** — 智能规划与决策相关研究。
- 🎮 **[move 控制原理](https://github.com/OpenHUTB/move)** — 运动控制与生物力学相关。

人车模拟器的技术架构如下图所示：

<a href="https://github.com/OpenHUTB/.github/blob/master/fig/repositories.md">
<img src="https://github.com/OpenHUTB/.github/blob/master/profile/repositories.png?raw=true" width="40%" >
</a>




<!--所有项目关系的思维导图。-->
<!-- 使用markmap进行编辑并生成svg：https://markmap.js.org/repl -->
<!-- 在profile/markmap.md中去保存图的数据 -->
<!-- svg图片预览：https://raw.githack.com/ -->

## 社区项目之间的关系

```mermaid
graph LR
    A[人的模型 <a href='https://github.com/OpenHUTB/opensim-core'>OpenSim</a>] --> B[多体物理 <a href='https://github.com/OpenHUTB/chrono'>chrono</a>]
    B --> C[<b>人车模拟器 <a href='https://github.com/OpenHUTB/hutb'>hutb</a> </b>]
    A --> F[<a href='https://github.com/MyoHub/myoconverter'>格式转换</a> <a href='https://github.com/OpenHUTB/mujoco_plugin'>mujoco_plugin</a> ]
    F --> C
    C --> D[文档 <a href='https://github.com/OpenHUTB/doc'>doc</a>]
    D --> H[无人机文档 <a href='https://github.com/OpenHUTB/air_doc'>air_doc</a>]
    D --> I[神经原理 <a href='https://github.com/OpenHUTB/neuro'>neuro</a>]
    I --> J[规划 <a href='https://github.com/OpenHUTB/PFC'>PFC</a>]
    I --> K[控制原理 <a href='https://github.com/OpenHUTB/move'>move</a>]
    K --> A
    L[模拟引擎 <a href='https://github.com/OpenHUTB/engine'>engine</a>] --> C
    L --> M[引擎文档 <a href='https://github.com/OpenHUTB/engine_doc'>engine_doc</a>]
    M --> S[C++ 文档 <a href='https://github.com/OpenHUTB/cpp'>cpp</a>]
    D --> M
    L --> N[无人机模拟器 <a href='https://github.com/OpenHUTB/air'>air</a>]
    N --> C
    N --> H
    D --> R[<a href='https://github.com/OpenHUTB/.github/blob/master/README.md#%E5%BA%94%E7%94%A8%E5%88%97%E8%A1%A8'>应用列表</a>]
    D --> Q[<a href='https://github.com/OpenHUTB/.github/blob/master/README.md#%E5%B7%A5%E5%85%B7%E5%88%97%E8%A1%A8'>工具列表</a>]


    style I fill:#e1f5fe
    style C fill:#ccffcc
    style D fill:#fff3e0
    style Q fill:#f3e5f5
    style R fill:#F5DEB3
```



### 应用列表

```mermaid
graph LR

    A --> F[人的移动 <a href='https://github.com/OpenHUTB/locomotion'>locomotion</a>]
    F --> L[人的模拟 <a href='https://github.com/OpenHUTB/carla-pedestrians'>carla-pedestrians</a>]

    A --> G[自动驾驶测试 <a href='https://github.com/OpenHUTB/platform'>platform</a>]
    G --> H[强化学习 <a href='https://github.com/OpenHUTB/carla_rl'>carla_rl</a>]
    H --> K[<a href='https://github.com/OpenHUTB/Carla_Autonomous_Driving'>Carla_Autonomous_Driving</a>]
    H --> I[模仿学习 <a href='https://github.com/OpenHUTB/carla-roach'>carla-roach</a>]
    H --> J[多视角 <a href='https://github.com/OpenHUTB/CILv2_multiview'>CILv2_multiview</a>]
    G --> M[安全场景生成 <a href='https://github.com/OpenHUTB/ChatScene'>ChatScene</a>]

    A[应用列表] --> B[智慧交通 <a href='https://github.com/OpenHUTB/intelligent_traffic/'>intelligent_traffic</a>]
    B --> C[交通孪生 <a href='https://github.com/OpenHUTB/traffic_twin/'>traffic_twin</a>]
    C --> N[轨迹跟踪 <a href='https://github.com/OpenHUTB/Self_Driving_Car_Trajectory_Tracking'>Trajectory_Tracking</a>]
    B --> D[模拟端 <a href='https://github.com/OpenHUTB/driving/'>driving</a> ]
    O --> E[交通大模型 <a href='https://github.com/OpenHUTB/traffic_llm'>traffic_llm</a>]
    B --> O[模型上下文协议 <a href='https://github.com/OpenHUTB/mcp'>mcp</a>]

    style A fill:#F5DEB3
```


### 工具列表

```mermaid
graph LR
    A[工具列表] --> B[<a href='https://github.com/OpenHUTB/latex'>latex</a> 模板]
    B --> C[课程设计 <a href='https://github.com/OpenHUTB/course'>course</a>]
    B --> D[研究生论文 <a href='https://github.com/OpenHUTB/master'>master</a>]
    B --> E[本科毕设 <a href='https://github.com/OpenHUTB/undergraduate'>undergraduate</a>]
    E --> M[<a href='https://github.com/OpenHUTB/powerpoint2pdf'>sim</a>]
    D --> N[<a href='https://github.com/OpenHUTB/emotion'>emotion</a>]
    G --> F[<a href='https://github.com/OpenHUTB/powerpoint2pdf'>powerpoint2pdf</a>]
    A --> G[工具脚本 <a href='https://github.com/OpenHUTB/utils'>utils</a>]
    A --> V[<a href='https://github.com/OpenHUTB/vsc'>vsc</a> 代码补全插件]
    G --> O[文档生成 <a href='https://github.com/OpenHUTB/mkdocs'>mkdocs</a>]
    G --> H[<a href='https://github.com/OpenHUTB/matlab'>matlab</a>]
    A --> K[<a href='https://github.com/OpenHUTB/ros'>ros</a>]
    K --> L[<a href='https://github.com/OpenHUTB/ros-bridge'>ros-bridge</a>]

    style A fill:#f3e5f5
```
