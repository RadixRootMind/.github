<div align="center">

<img src="assets/logo.png" alt="RadixRootMind logo" width="130">

# 🌳 RadixRootMind

**Chip-rooted open infrastructure for on-device embodied intelligence**

*Turning frontier research into open models, systems, data, and evaluation — from silicon up to real-world physical intelligence.*

[![GitHub followers](https://img.shields.io/github/followers/RadixRootMind?style=social)](https://github.com/RadixRootMind)
[![Awesome](https://awesome.re/badge.svg)](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/RadixRootMind)

**English** · [中文](#-中文)

</div>

---

We are an open developer organization building the **compute substrate for embodied AI** — the layer that connects low-level chip capability, hardware-aware optimization, quantization, and edge deployment to real robots acting in the physical world. Think of it as an **open, chip-rooted foundation** for Vision-Language-Action (VLA) and World-Action (WAM) models — interoperable with existing kernel/compiler ecosystems, not a walled garden.

## 🚀 Available now

| Project | What it is | Status |
|---|---|---|
| [**Awesome-Quant-VLA-WAM**](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM) | Curated reading list — 180+ papers on quantization for VLA & World-Action models, with a five-category taxonomy, roadmap, and evaluation guide | ✅ **Live** |
| **quant-vla** | Companion engineering stack: VLA post-training quantization (W4A4 & more) + LIBERO evaluation, reproducible pipeline | 🚧 **Coming soon** |

> New here? Start with the **Awesome list** above — ⭐ star & watch to follow the first code release.

## 🧭 What we're building

Maturity: ✅ available · 🚧 in progress · 🗺️ planned

**⚡ VLA Quantization & Inference Engine** — 🚧
End-to-end perception → understanding → prediction → planning → decision; W4A4 and other formats; unified multimodal streaming for low-latency, high-throughput inference.

**📊 Evaluation & Deployment Tools** — 🚧
Benchmarks (LIBERO, ManiSkill2/3, OpenVLA-Bench, WorldReasonBench …); data standards (RLDS, Open-X Embodiment); Studio for model discovery, GPU allocation, and `torchrun` distributed launch; visualization + end-to-end deploy chain.

**🌉 Cross-chip Unified Adaptation Layer** — 🗺️
Unified operator interface & heterogeneous scheduling; high-performance kernel library; hardware-aware optimization that auto-generates optimal code.

**⚙️ MLIR Compilation Infrastructure** — 🗺️
Full graph-lowering & codegen toolchain; Triton-kernel auto-registration & compile caching; dynamic batching & multi-GPU sequence parallelism.

**🤖 Motion — Robot Motion Control** — 🗺️
Streaming temporal inference + multimodal motion control; millisecond real-time control loop; closed-loop feedback & policy deployment.

**🌍 World Models & On-chip Security** — 🗺️
WAM adaptation & predictive inference; trusted boot, data encryption, privacy; on-chip autonomy auditing & governance.

## 🗺️ Roadmap

- **Phase 0 — Foundations** *(now)*: research list, org profile, community setup (WeChat group + contribution guides).
- **Phase 1 — First code drop**: open-source `quant-vla` with a reproducible *quantize → LIBERO → numbers* pipeline + demo.
- **Phase 2 — Light up the pillars**: ship one pillar at a time (engine → eval/deploy → cross-chip → MLIR → motion → WAM).
- **Phase 3 — Ecosystem**: chip-vendor & institutional partnerships, real-robot demos, contributor programs.

## 🤝 Who we're looking for

💻 Quantization / compiler / inference engineers · 🔬 VLA & world-model researchers · 🤖 robotics application developers · 🏢 chip vendors & institutional partners

## 🙌 How to Contribute

All contributions are welcome — no change is too small.

- 📚 **Add a paper / benchmark** to [Awesome-Quant-VLA-WAM](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM): open a PR following the table format (title · type · link), or just open an Issue with the link and we'll add it.
- 🐛 **Report bugs or gaps** — open an Issue describing what's wrong or missing.
- 🔬 **Share results** — reproduction numbers, new quantization routes, or ablations.
- 📝 **Improve docs** — fix typos, clarify wording, or translate.
- 💡 **Propose ideas** — start a discussion or open an Issue for new directions.

**Workflow:** Fork → branch → make your change → open a Pull Request. For anything larger, open an Issue first so we can align. Keep PRs focused with a short description, and please be respectful and constructive.

New here? Look for issues labeled **`good first issue`**.

## ⭐ Get involved

- **Star & watch** the repos to follow releases
- Open **Issues / PRs** — feedback, papers, and benchmarks all welcome
- 📧 **xuenaier856@gmail.com** · 🐙 [github.com/RadixRootMind](https://github.com/RadixRootMind) · 💬 WeChat (below)

---

## 🌳 中文

**根植于芯片的开放基础设施,服务端侧具身智能。**

RadixRootMind 是一个开放开发者组织,致力于打造**具身智能的算力底座**——打通芯片底层能力、硬件感知优化、量化与边缘部署,直到真机在物理世界中执行动作。我们为 VLA(视觉-语言-动作)与 WAM(世界-动作)模型提供**根植于芯片的开放基座**,并与现有算子/编译器生态互通。

### 🚀 现已开放

| 项目 | 简介 | 状态 |
|---|---|---|
| [**Awesome-Quant-VLA-WAM**](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM) | 精选论文合集——180+ 篇 VLA & 世界模型量化研究,含五大分类体系、roadmap 与评测指南 | ✅ **已上线** |
| **quant-vla** | 配套工程栈:VLA 后训练量化(W4A4 等)+ LIBERO 评测,可复现 pipeline | 🚧 **即将开源** |

>  **Awesome 合集**——⭐ Star & Watch 关注首个代码发布。

### 🧭 主要工作方向

成熟度:✅ 已开放 · 🚧 开发中 · 🗺️ 规划中

- **⚡ VLA 量化与推理引擎** — 🚧 感知/理解/预测/规划/决策端到端;W4A4 等多格式;统一多模态流式,低延迟高吞吐
- **📊 评测与部署工具** — 🚧 LIBERO、ManiSkill2/3、OpenVLA-Bench、WorldReasonBench 等;RLDS、Open-X Embodiment;Studio(模型发现、GPU 分配、torchrun 分布式启动);可视化 + 端到端部署链
- **🌉 跨芯片统一适配层** — 🗺️ 统一算子接口与异构调度;高性能算子库;硬件感知优化自动生成最优代码
- **⚙️ MLIR 编译基础设施** — 🗺️ 完整图降级与代码生成;Triton kernel 自动注册与编译缓存;动态批处理与多 GPU 序列并行
- **🤖 Motion 机器人运动控制** — 🗺️ 流式时序推理 + 多模态运动控制;毫秒级实时控制循环;闭环反馈与策略部署
- **🌍 世界模型与片上安全** — 🗺️ WAM 适配加速与预测推理;可信启动、数据加密、隐私保护;片上自主性审计与治理

### 🤝 欢迎加入

💻 量化/编译/推理开发者 · 🔬 VLA/世界模型研究者 · 🤖 机器人应用开发者 · 🏢 芯片厂商与机构合作伙伴

### 🙌 如何贡献

欢迎任何形式的贡献,再小也欢迎:

- 📚 **补充论文 / benchmark** 到 [Awesome-Quant-VLA-WAM](https://github.com/RadixRootMind/Awesome-Quant-VLA-WAM):按表格格式(标题 · 类型 · 链接)提 PR;或直接开 Issue 贴链接,我们来加。
- 🐛 **报告问题 / 缺漏** —— 开 Issue 说明哪里有误或缺失。
- 🔬 **分享结果** —— 复现数据、新量化路线、消融实验。
- 📝 **完善文档** —— 改错别字、优化措辞、翻译。
- 💡 **提出想法** —— 发起 Discussion 或开 Issue 讨论新方向。

**流程**:Fork → 建分支 → 修改 → 提 Pull Request;较大改动请先开 Issue 对齐。PR 请保持聚焦并简要说明,友善建设性沟通。

新人可从标记 **`good first issue`** 的 issue 入手。

⭐ 欢迎 Star 支持,Issues / PR / 反馈都欢迎!
📧 xuenaier856@gmail.com · 🐙 github.com/RadixRootMind · 💬 微信见下

---

## 💬 Community · 社区

<div align="center">
<b>WeChat · 微信</b><br/>
<sub>加好友进「RadixRootMind 中国区开发者」群</sub><br/><br/>
<img src="assets/wechat.png" alt="WeChat QR — add to join the developer group" width="220"/><br/>
<sub>扫码加发起人,备注 <code>RadixRootMind</code> 拉你进群</sub>
</div>
