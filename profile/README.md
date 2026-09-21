<div align="center">

# RadixRootMind

**Chip-grounded open infrastructure for on-device embodied intelligence**

[![Awesome](https://awesome.re/badge.svg)](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/RadixRootMind)

**English** · [中文](#中文)

</div>

---

RadixRootMind is an open research and engineering organization focused on **chip-grounded infrastructure for on-device embodied intelligence** — spanning cross-chip operator-library adaptation, hardware-aware optimization, quantization, MLIR-based compilation, multimodal streaming inference, edge runtimes, closed-loop robotic motion control, edge-cloud collaborative orchestration, communication-sensing-computing fusion networks, cloud robot brain platforms, world-model prediction, and trusted on-device autonomy.

We turn research insight into open models, compiler toolchains, inference engines, control systems, datasets, and evaluation frameworks — connecting chip-level capability up to real-world physical intelligence. Everything is built in the open and designed to interoperate with existing operator libraries, compiler stacks (Triton / MLIR), and robotics middleware (ROS 2), for the broader AI, robotics, and semiconductor communities.

## Projects

| Project | Description | Status |
|---|---|---|
| [**Awesome-Quant-VLA-WAM**](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM) | A curated list of 180+ papers on quantization for Vision-Language-Action (VLA) and World-Action (WAM) models — compressing large embodied policies to low bit-widths while keeping robots able to act. Includes transferred LLM/DiT baselines, VLA-specific PTQ/QAT, deployment routes, and WAM extensions. | ✅ Available |
| [**RadixQuantVLA**](https://github.com/RadixRootMind/RadixQuantVLA) | A Lego-like framework for unified quantization and deployment of VLA models. Integrates QuantVLA, Ω-QVLA, QVLA/OpenVLA, OpenVLA-OFT, UniVLA, StarVLA, GR00T-N1.5, and Pi0.5/OpenPI routes behind shared launchers, checkpoint conventions, and validation pipelines. | 🚀 Active Development |
| [**Radix-Embodied-Stack**](https://github.com/RadixRootMind/Radix-Embodied-Stack) | Universal infrastructure for embodied AI: cross-model, cross-chip, cross-platform deployment of VLA/VLM+Policy/Diffusion Policy/WAM on domestic chips. Covers model quantization, inference runtime with hardware adaptation, and multi-robot control interfaces. | 📋 Planned |

## Technical Directions

Nine directions at different stages of maturity, spanning chip-level infrastructure to cloud-edge-device orchestration for embodied intelligence.

**1. Cross-chip Operator-Library Adaptation** *(in progress)*
A unified operator interface and heterogeneous scheduling layer across domestic and mainstream accelerators (GPU, DCU, NPU, and compute-in-memory devices). Rather than re-implementing kernels, we adapt and reuse open operator libraries and generate hardware-aware kernels, with a capability-abstraction layer that shields chip-specific differences from the layers above.

**2. MLIR Compilation Infrastructure** *(planned)*
An end-to-end graph-lowering and code-generation toolchain: operator fusion, Triton-kernel auto-registration and compile caching, dynamic batching, and multi-GPU sequence parallelism — bridging model graphs to portable, hardware-specific executables.

**3. VLA Quantization and Inference Engine** *(in progress)*
A low-bit inference engine for embodied policies: quantized (W4A4 and mixed-precision) linear and attention kernels, KV-cache quantization, action-token decoding, and unified multimodal streaming for low-latency, high-throughput closed-loop inference. Grounded in post-training quantization (PTQ) and quantization-aware training (QAT) methods that preserve action fidelity, not only layer-output error.

**4. Motion Control — A-Motion, ROS 2** *(planned)*
A real-time control stack that couples streaming temporal inference with multimodal motion control. The A-Motion closed loop targets millisecond-scale control frequencies, closed-loop feedback, and policy deployment on real robots, integrated with ROS 2 for perception, actuation, and system orchestration.

**5. World Models and On-chip Security** *(planned)*
World-Action-Model (WAM) adaptation and predictive inference for embodied decision-making; trusted boot, data encryption, and privacy protection; on-chip autonomy auditing and governance.

**6. Evaluation and Deployment Tools** *(in progress)*
Reproducible closed-loop evaluation on standard benchmarks (LIBERO, ManiSkill2/3, SimplerEnv, OpenVLA-Bench); data standards (RLDS, Open-X Embodiment); model discovery, resource allocation, and distributed launch; visualization and an end-to-end deployment chain.

**7. Device-Edge-Cloud Collaborative Framework** *(planned)*
A unified communication-compute-control (3C) framework spanning single embodied agents to multi-robot clusters. End-edge-cloud three-tier architecture for streaming perception fusion, distributed inference offload, and coordinated motion planning — bridging on-device autonomy with cloud-scale intelligence.

**8. Edge Communication-Sensing-Computing Network** *(planned)*
A fusion network stack integrating NearLink/5G communications with deterministic low-latency routing, multimodal sensor streaming, and self-organizing mesh networking — enabling real-time sensory data flow and compute orchestration at the edge.

**9. Cloud Robot Brain Platform** *(planned)*
A centralized orchestration and scheduling platform for embodied agent fleets: multi-robot task planning, elastic compute allocation, cloud-hosted inference services, and closed-loop data collection — aggregating fleet experience and distributing intelligence back to edge devices.

## Roadmap

- **Phase 0 — Foundations** *(current)*: research list, organization profile, and community setup.
- **Phase 1 — First code release**: open-source `RadixQuantVLA` with a reproducible quantize–evaluate–report pipeline.
- **Phase 2 — Build out the stack**: deliver directions 1-6 (chip adaptation, compilation, inference, motion control, evaluation, world models) one at a time.
- **Phase 3 — Edge-cloud orchestration**: deliver directions 7-9 (device-edge-cloud collaboration, fusion networks, cloud robot brain).
- **Phase 4 — Ecosystem**: chip-vendor and institutional partnerships, real-robot demonstrations, and contributor programs.

## Join RadixRootMind

🚀 **RadixRootMind is recruiting passionate developers and tech enthusiasts!** If you're excited about the foundational stack for embodied intelligence, join us in building the domestic "Compute-Communication-Control" fusion ecosystem.

### 🔥 Core Maintainers

**We're looking for:**
- Deep expertise in embodied-intelligence system architecture, communication-sensing-computing fusion, real-time control, or edge computing
- Master's degree (or exceptional bachelor's) in Computer Science, Automation, Robotics, EE, or Communications
- Commitment to long-term ownership of a technical module (e.g., low-power operator libraries, deterministic network stacks, motion-control loops, hardware abstraction layers)
- Ability to propose innovative solutions and push the boundaries of "3C fusion" technology

**What you'll gain:**
- Official contributor certification and digital certificate
- Long-term career development support and academic resource access
- Technical content exposure on RadixRootMind official channels (papers, enterprise brand)
- Your code and solutions prioritized for mainline integration and public showcase
- Opportunity to lead or co-organize tech meetups, hackathons, and offline events
- Open commercialization pathways — deep participation in ecosystem partner projects with revenue sharing
- Potential to become a RadixRootMind ecosystem partner

### 🌱 Community Contributors

**We're looking for:**
- Believers in open source who care about the embodied-intelligence industry and want to contribute to the community
- Strengths in community work: technical blogging, open-source evangelism, developer community management, or event planning
- Bachelor's degree or above — any major welcome; we value your unique skills and passion

**What you'll gain:**
- Official community contributor certification and digital certificate
- Early access to major community events
- Exposure to media, industry leaders, and technical experts
- Internal referral track — priority for internships and full-time roles at ecosystem partners
- Your contributions promoted and credited across RadixRootMind platforms
- High performers may become ecosystem partners

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

RadixRootMind 是一个开放的研究与工程组织,聚焦**根植于芯片的端侧具身智能基础设施**——涵盖跨芯片算子库适配、硬件感知优化、量化、基于 MLIR 的编译、多模态流式推理、边缘运行时、闭环机器人运动控制、端-边-云协同编排、通感智算融合网络、云端机器人大脑平台、世界模型预测,以及可信的端侧自主性。

我们把研究洞见转化为开放的模型、编译工具链、推理引擎、控制系统、数据集与评测框架,打通从芯片底层能力到真实物理智能的完整链路。所有工作均以开放方式构建,并与现有算子库、编译栈(Triton / MLIR)、机器人中间件(ROS 2)互通,服务于更广泛的 AI、机器人与半导体社区。

### 项目

| 项目 | 简介 | 状态 |
|---|---|---|
| [**Awesome-Quant-VLA-WAM**](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM) | 精选 180+ 篇 VLA(视觉-语言-动作)与 WAM(世界-动作)模型量化论文清单——将大型具身策略压缩至低比特宽度的同时保持机器人行动能力。包含迁移的 LLM/DiT 基线、VLA 专用 PTQ/QAT、部署路线与 WAM 扩展。 | ✅ 已上线 |
| [**RadixQuantVLA**](https://github.com/RadixRootMind/RadixQuantVLA) | 统一的 VLA 模型量化与部署框架,如同乐高积木。整合 QuantVLA、Ω-QVLA、QVLA/OpenVLA、OpenVLA-OFT、UniVLA、StarVLA、GR00T-N1.5、Pi0.5/OpenPI 等路线,共享启动器、检查点规范与验证流程。 | 🚀 活跃开发中 |
| [**Radix-Embodied-Stack**](https://github.com/RadixRootMind/Radix-Embodied-Stack) | 具身 AI 通用基础设施:跨模型、跨芯片、跨平台部署 VLA/VLM+Policy/Diffusion Policy/WAM 到国产芯片。涵盖模型量化、硬件适配的推理运行时、多机器人控制接口。 | 📋 规划中 |

### 技术方向

九个方向,处于不同成熟度阶段,从芯片底层基础设施到端-边-云协同编排,覆盖具身智能全栈。

**1. 跨芯片统一适配**(开发中)
面向国产与主流加速器(GPU、DCU、NPU、存算一体等)的统一算子接口与异构调度层。不重复造轮子,而是适配并复用开放算子库、生成硬件感知的高性能 kernel,并以能力抽象层向上屏蔽芯片差异。

**2. MLIR 编译工具链**(规划中)
端到端的图降级与代码生成工具链:算子融合、Triton kernel 自动注册与编译缓存、动态批处理、多 GPU 序列并行——把模型计算图桥接到可移植、面向具体硬件的可执行文件。

**3. 具身模型量化与推理**(开发中)
面向具身策略的低比特推理引擎:量化(W4A4 与混合精度)的线性与注意力算子、KV-cache 量化、动作 token 解码,以及统一多模态流式,实现低延迟、高吞吐的闭环推理。以保持动作保真度(而非仅层输出误差)的后训练量化(PTQ)与量化感知训练(QAT)方法为基础。

**4. Motion 运动控制**(规划中)
将流式时序推理与多模态运动控制耦合的实时控制栈。A-Motion 闭环面向毫秒级控制频率、闭环反馈与真机策略部署,并与 ROS 2 集成完成感知、执行与系统编排。

**5. 世界模型 & 片上安全**(规划中)
面向具身决策的 WAM 适配与预测推理;可信启动、数据加密与隐私保护;片上自主性审计与治理。

**6. 评测 + 部署工具**(开发中)
在标准 benchmark(LIBERO、ManiSkill2/3、SimplerEnv、OpenVLA-Bench)上的可复现闭环评测;数据标准(RLDS、Open-X Embodiment);模型发现、资源分配与分布式启动;可视化与端到端部署链。

**7. 从单体到集群:通感智算融合**(规划中)
统一的通信-计算-控制(3C)框架,覆盖单个具身智能体到多机器人集群。端-边-云三级架构,支持流式感知融合、分布式推理卸载与协同运动规划——打通端侧自主与云端智能。

**8. 边缘通感智算融合网络**(规划中)
融合星闪/5G 通信的网络栈,支持确定性低时延路由、多模态传感器流与自组织组网——在边缘层实现实时感知数据流动与算力编排。

**9. 云端集群调度平台(Cloud Robot Brain)**(规划中)
具身智能体集群的中心化编排与调度平台:多机任务规划、弹性算力分配、云端推理服务与闭环数据回流——汇聚集群经验并将智能分发回边缘设备。

### 加入 RadixRootMind 开源社区

🚀 **RadixRootMind 正在召集志同道合的开发者与技术爱好者！** 如果你对具身智能底层技术栈充满热情,欢迎与我们携手打造国产具身智能"计算-通信-控制"融合生态。

#### 🔥 开源项目维护者(Core Maintainer)

**我们在寻找这样的你:**
- 深耕于具身智能系统架构、通感算融合、实时控制、边缘计算等技术领域
- 拥有计算机、自动化、机器人、电子、通信等相关专业研究生学位(本科背景优秀者亦可考虑)
- 愿意长期投入某一技术模块的迭代与维护(例如:低功耗算子库、确定性通信栈、运动控制闭环、硬件抽象层等)
- 善于提出创新解决方案,推动"3C 融合"技术边界拓展

**加入我们,你将获得:**
- 官方认证的开源贡献者身份及电子证书
- 长期的职业发展支持与学术资源对接
- 在 RadixRootMind 官方渠道的技术内容曝光(包括论文成果、企业技术品牌)
- 你的代码与方案将被优先集成到主分支并公开展示
- 有机会主导或联合发起技术 Meetup、黑客松等线下活动
- 开放商业化合作通道,深度参与生态伙伴项目并分享收益
- 有机会成为 RadixRootMind 生态合伙人

#### 🌱 社区志愿者(Community Contributor)

**我们在寻找这样的你:**
- 认同开源理念,关注具身智能产业发展,愿意为社区生态添砖加瓦
- 擅长某一类社区工作,例如:技术博客创作、开源项目传播、开发者社群维护、活动策划执行等
- 本科及以上学历,专业不限——我们重视你的独特技能与热情

**加入我们,你将获得:**
- 社区志愿者官方认证及数字证书
- 提前参与社区重要活动的资格
- 接触媒体、产业、技术专家等多元化资源
- 内推通道:生态伙伴的实习与全职岗位优先推荐
- 你的贡献将在 RadixRootMind 全平台获得传播与署名
- 表现优异者有机会成为生态合伙人

### 路线图

- **Phase 0 — 基础阶段**(当前):研究清单、组织主页与社区搭建。
- **Phase 1 — 首次代码发布**:开源 `RadixQuantVLA`,提供可复现的量化–评测–报告流程。
- **Phase 2 — 构建端侧技术栈**:逐步交付方向 1-6(芯片适配、编译、推理、运动控制、评测、世界模型)。
- **Phase 3 — 边-云协同编排**:交付方向 7-9(端-边-云协同、融合网络、云端机器人大脑)。
- **Phase 4 — 生态建设**:芯片厂商与机构合作、真机演示与贡献者计划。

### 如何贡献

欢迎任何形式的贡献,再小也欢迎:

- **补充论文 / benchmark** 到 [Awesome-Quant-VLA-WAM](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM):按表格格式提 PR,或开 Issue 贴链接。
- **报告问题 / 缺漏**:开 Issue 说明哪里有误或缺失。
- **分享结果**:复现数据、新量化路线、消融实验。
- **完善文档**:修订、优化措辞或翻译。
- **提出想法**:开 Issue 或发起 Discussion 讨论新方向。

流程:Fork、建分支、修改、提 Pull Request;较大改动请先开 Issue 对齐。新人可从标记 `good first issue` 的 issue 入手。

**申请成为开源项目维护者或社区志愿者,请发邮件至 xuenaier856@gmail.com 并附上简历及贡献意向。**

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
