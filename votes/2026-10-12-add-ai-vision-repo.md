# 申请创建 ai-vision 代码仓库 to ob-labs

## 项目基本信息

**项目名称：** ai-vision（AI Vision）

**项目目的：**

ai-vision 是面向个人和团队的开源 AI Agent 观测与诊断平台。通过采集插件和 SDK 接入，统一查看 Agent 的执行轨迹、模型调用、工具执行和多轮会话，提供 Token 用量与成本分析、自动诊断及质量看板，帮助开发者理解任务如何完成、问题出在哪里、资源消耗在哪里，并依据实际运行记录改进 Agent 的质量与效率。

在 OceanBase 开源生态中的价值包括：

- **补充 AI 应用的观测与诊断能力：** 围绕 [SIG AI](https://oceanbase.github.io/docs/sig/AI/sig_intro) 推动数据库与 AI 融合的方向，为 Coding Agent、个人助手及企业智能体提供运行分析工具，支持从问题发现、轨迹复查到效果改进的完整流程。
- **拓展 OceanBase 在 Agent 场景中的应用：** 整套部署默认使用 OceanBase CE，也可复用已有 OceanBase 实例，为社区提供 Agent 运行数据管理与诊断分析的工程实践。
- **连接主流 Agent 生态：** 支持 Claude Code、Codex、OpenClaw、OpenCode 等应用接入，采用 OpenTelemetry / OTLP 采集链路，并提供 Langfuse SDK 轨迹上报与部分查询接口兼容能力，方便已有应用沿用埋点接入。
- **提供可扩展的诊断能力：** 通过 AgentLens 诊断引擎，在采集数据支持的范围内检查工具失败、重复调用、反复改写和耗时异常等问题，并将诊断结果关联至原始轨迹，方便开发者复查和扩展诊断规则。
- **降低社区使用门槛：** 提供中文界面、Docker / Kubernetes 私有化部署，以及 `aiv` CLI 和部署、查询 Skill，支持个人体验与团队使用。

**仓库地址：**

仓库地址：<https://github.com/ob-labs/ai-vision-ob>

**代码现状：**

当前代码托管于 [ob-labs/ai-vision-ob](https://github.com/ob-labs/ai-vision-ob)，采用 monorepo 组织，已包含平台前后端、AgentLens 诊断引擎、Antcollector 采集服务、Agent 接入插件、CLI 与相关 Skill。

项目已具备采集接入、执行轨迹查看、用量分析和诊断能力，并提供安装部署、使用及源码构建文档，相关能力持续迭代完善中。

**项目责任人（GitHub ID）：**

- Maintainer: webup

**开源协议：**

Apache License 2.0，当前仓库已包含相应 `LICENSE` 文件。

## 开源项目检查清单

> 检查清单旨在规范项目，方便社区用户使用。尚未完成的内容应在项目创建后尽快补充。

- [x] 包含 README.md，并提供中文说明。
- [ ] 包含 CONTRIBUTING.md，可参考 OceanBase 社区 [CONTRIBUTING 文件](https://github.com/oceanbase/.github/blob/main/CONTRIBUTING.md)。
- [ ] 包含 CODE_OF_CONDUCT.md；未单独提供时使用 OceanBase 社区现有的[行为准则文件](https://github.com/oceanbase/.github/blob/main/CODE_OF_CONDUCT.md)。
- [x] 包含用户安装指导说明，提供 Docker / Kubernetes 部署文档。
- [x] 包含用户使用指导说明，覆盖 Agent 接入、轨迹查看及 CLI 查询等操作。
- [x] 包含源码构建指导说明，提供源码部署入口及相关组件开发文档。

## 投票截止时间

如果不满足投票条件，此投票将在 2026 年 10 月 25 日截止。

> 满足投票条件是说投票已经成功，比如已经有不少于 2/3 的 TOC 投票，或者投票失败，比如有一半的 TOC 反对。

## 投票结果

参考 [申请 创建 AI Vision 项目](https://github.com/oceanbase/community/pull/90)。