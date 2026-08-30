<div align="center">

# RadixRootMind

**Chip-grounded open infrastructure for on-device embodied intelligence**

[![Awesome](https://awesome.re/badge.svg)](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/RadixRootMind)

**English** · [中文](#中文)

</div>

---

RadixRootMind is an open research and engineering organization focused on **chip-grounded infrastructure for on-device embodied intelligence** — spanning cross-chip operator-library adaptation, hardware-aware optimization, quantization, MLIR-based compilation, multimodal streaming inference, edge runtimes, closed-loop robotic motion control, world-model prediction, and trusted on-device autonomy.

We turn research insight into open models, compiler toolchains, inference engines, control systems, datasets, and evaluation frameworks — connecting chip-level capability up to real-world physical intelligence. Everything is built in the open and designed to interoperate with existing operator libraries, compiler stacks (Triton / MLIR), and robotics middleware (ROS 2), for the broader AI, robotics, and semiconductor communities.

## Projects

| Project | Description | Status |
|---|---|---|
| [**Awesome-Quant-VLA-WAM**](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM) | Curated reading list of 180+ papers on quantization for Vision-Language-Action (VLA) and World-Action (WAM) models, with a five-category taxonomy and an evaluation guide | Available |
| **quant-vla** | Companion engineering stack for VLA post-training quantization (W4A4 and beyond) with LIBERO evaluation and a reproducible pipeline | In preparation |

## Technical Directions

Six directions at different stages of maturity, each targeting a concrete layer of the on-device embodied stack.

**Cross-chip Operator-Library Adaptation** *(planned)*
A unified operator interface and heterogeneous scheduling layer across domestic and mainstream accelerators (GPU, DCU, NPU, and compute-in-memory devices). Rather than re-implementing kernels, we adapt and reuse open operator libraries and generate hardware-aware kernels, with a capability-abstraction layer that shields chip-specific differences from the layers above.

**VLA Quantization and Inference Engine** *(in progress)*
A low-bit inference engine for embodied policies: quantized (W4A4 and mixed-precision) linear and attention kernels, KV-cache quantization, action-token decoding, and unified multimodal streaming for low-latency, high-throughput closed-loop inference. Grounded in post-training quantization (PTQ) and quantization-aware training (QAT) methods that preserve action fidelity, not only layer-output error.

**MLIR Compilation Infrastructure** *(planned)*
An end-to-end graph-lowering and code-generation toolchain: operator fusion, Triton-kernel auto-registration and compile caching, dynamic batching, and multi-GPU sequence parallelism — bridging model graphs to portable, hardware-specific executables.

**Closed-loop Motion Control — A-Motion, ROS 2** *(planned)*
A real-time control stack that couples streaming temporal inference with multimodal motion control. The A-Motion closed loop targets millisecond-scale control frequencies, closed-loop feedback, and policy deployment on real robots, integrated with ROS 2 for perception, actuation, and system orchestration.

**Evaluation and Deployment Tools** *(in progress)*
Reproducible closed-loop evaluation on standard benchmarks (LIBERO, ManiSkill2/3, SimplerEnv, OpenVLA-Bench); data standards (RLDS, Open-X Embodiment); model discovery, resource allocation, and distributed launch; visualization and an end-to-end deployment chain.

**World Models and On-chip Security** *(planned)*
World-Action-Model (WAM) adaptation and predictive inference for embodied decision-making; trusted boot, data encryption, and privacy protection; on-chip autonomy auditing and governance.

## Roadmap

- **Phase 0 — Foundations** *(current)*: research list, organization profile, and community setup.
- **Phase 1 — First code release**: open-source `quant-vla` with a reproducible quantize–evaluate–report pipeline.
- **Phase 2 — Build out the stack**: deliver one direction at a time (inference engine, evaluation and deployment, operator-library adaptation, MLIR, motion control, world models).
- **Phase 3 — Ecosystem**: chip-vendor and institutional partnerships, real-robot demonstrations, and contributor programs.

## Who We're Looking For

Quantization, compiler, and inference engineers; VLA and world-model researchers; robotics and ROS developers; and chip-vendor and institutional partners.

## Contributing

Contributions of any size are welcome.

- **Add a paper or benchmark** to [Awesome-Quant-VLA-WAM](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM): open a pull request following the table format, or open an issue with the link.
- **Report bugs or gaps** by opening an issue.
- **Share results** — reproduction numbers, new quantization routes, or ablations.
- **Improve documentation** — corrections, clearer wording, or translations.
- **Propose ideas** — open an issue or a discussion for new directions.

Workflow: fork, branch, make your change, and open a pull request. For larger changes, open an issue first. New contributors can start with issues labeled `good first issue`.

## Contact

- Email: xuenaier856@gmail.com
- GitHub: [github.com/RadixRootMind](https://github.com/RadixRootMind)
- WeChat: see below

---

## 中文

**根植于芯片的开放基础设施,服务端侧具身智能。**

RadixRootMind 是一个开放的研究与工程组织,聚焦**根植于芯片的端侧具身智能基础设施**——涵盖跨芯片算子库适配、硬件感知优化、量化、基于 MLIR 的编译、多模态流式推理、边缘运行时、闭环机器人运动控制、世界模型预测,以及可信的端侧自主性。

我们把研究洞见转化为开放的模型、编译工具链、推理引擎、控制系统、数据集与评测框架,打通从芯片底层能力到真实物理智能的完整链路。所有工作均以开放方式构建,并与现有算子库、编译栈(Triton / MLIR)、机器人中间件(ROS 2)互通,服务于更广泛的 AI、机器人与半导体社区。

### 项目

| 项目 | 简介 | 状态 |
|---|---|---|
| [**Awesome-Quant-VLA-WAM**](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM) | 精选论文合集,180+ 篇 VLA(视觉-语言-动作)与 WAM(世界-动作)模型量化研究,含五大分类体系与评测指南 | 已上线 |
| **quant-vla** | 面向 VLA 后训练量化(W4A4 及更低)与 LIBERO 评测的配套工程栈,提供可复现 pipeline | 筹备中 |

### 技术方向

六个方向,处于不同成熟度阶段,分别对应端侧具身栈的一个具体层次。

**跨芯片算子库适配**(规划中)
面向国产与主流加速器(GPU、DCU、NPU、存算一体等)的统一算子接口与异构调度层。不重复造轮子,而是适配并复用开放算子库、生成硬件感知的高性能 kernel,并以能力抽象层向上屏蔽芯片差异。

**VLA 量化与推理引擎**(开发中)
面向具身策略的低比特推理引擎:量化(W4A4 与混合精度)的线性与注意力算子、KV-cache 量化、动作 token 解码,以及统一多模态流式,实现低延迟、高吞吐的闭环推理。以保持动作保真度(而非仅层输出误差)的后训练量化(PTQ)与量化感知训练(QAT)方法为基础。

**MLIR 编译基础设施**(规划中)
端到端的图降级与代码生成工具链:算子融合、Triton kernel 自动注册与编译缓存、动态批处理、多 GPU 序列并行——把模型计算图桥接到可移植、面向具体硬件的可执行文件。

**闭环运动控制 —— A-Motion,ROS 2**(规划中)
将流式时序推理与多模态运动控制耦合的实时控制栈。A-Motion 闭环面向毫秒级控制频率、闭环反馈与真机策略部署,并与 ROS 2 集成完成感知、执行与系统编排。

**评测与部署工具**(开发中)
在标准 benchmark(LIBERO、ManiSkill2/3、SimplerEnv、OpenVLA-Bench)上的可复现闭环评测;数据标准(RLDS、Open-X Embodiment);模型发现、资源分配与分布式启动;可视化与端到端部署链。

**世界模型与片上安全**(规划中)
面向具身决策的 WAM 适配与预测推理;可信启动、数据加密与隐私保护;片上自主性审计与治理。

### 欢迎加入

量化 / 编译 / 推理开发者、VLA 与世界模型研究者、机器人与 ROS 开发者,以及芯片厂商与机构合作伙伴。

### 如何贡献

欢迎任何形式的贡献,再小也欢迎:

- **补充论文 / benchmark** 到 [Awesome-Quant-VLA-WAM](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM):按表格格式提 PR,或开 Issue 贴链接。
- **报告问题 / 缺漏**:开 Issue 说明哪里有误或缺失。
- **分享结果**:复现数据、新量化路线、消融实验。
- **完善文档**:修订、优化措辞或翻译。
- **提出想法**:开 Issue 或发起 Discussion 讨论新方向。

流程:Fork、建分支、修改、提 Pull Request;较大改动请先开 Issue 对齐。新人可从标记 `good first issue` 的 issue 入手。

### 联系

- 邮箱:xuenaier856@gmail.com
- GitHub:github.com/RadixRootMind
- 微信:见下方

---

## Community · 社区

<div align="center">
<b>WeChat · 微信</b><br/>
<sub>加好友进「RadixRootMind 中国区开发者」群</sub><br/><br/>
<img src="assets/wechat.png" alt="WeChat QR" width="220"/><br/>
<sub>扫码加发起人,备注 <code>RadixRootMind</code> 拉你进群</sub>
</div>

---

<div align="center"><sub>Radix Root-layer Infrastructure for Chip-grounded On-device Embodied Intelligence</sub></div>
