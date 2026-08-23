# 申请创建 powercontext-ts 项目

## 项目基本信息

项目名称：powercontext-ts

建议仓库地址：<https://github.com/ob-labs/powercontext-ts>

### 项目目的

powercontext-ts 用于建设 PowerContext 面向 TypeScript 和 Node.js 生态的实现。项目以现有 [PowerContext Python 实现](https://github.com/oceanbase/powercontext)作为语义参考，通过受控的契约同步和跨语言一致性测试保持兼容；它不是对 Python 代码的逐行翻译，当前阶段也不立即替代 Python reference implementation。

项目首先交付可独立使用的 TypeScript Protocol 包和强类型 HTTP Client，使 TypeScript/JavaScript 应用能够直接调用 PowerContext Server；后续根据阶段验收结果，逐步建设 Core SDK、Node.js 本地 Runtime、Server、MCP、CLI 及完整产品能力。

同时，本项目也将作为未来评估 PowerContext 主体实现从 Python 向 TypeScript 演进的前期基础和技术探索载体。项目将通过跨语言契约、功能一致性、运行时能力、数据库兼容、部署运维和发布治理等方面的实际验证，为后续是否迁移、迁移到什么范围以及如何平滑迁移提供工程依据。

### 解决的问题

- 为 TypeScript/JavaScript 开发者提供官方、强类型且经过运行时验证的 PowerContext 访问方式，避免各 Node.js 宿主重复维护通用 HTTP Client 和协议类型。
- 降低 Node.js Agent、MCP 工具、编辑器扩展和 Web tooling 使用 PowerContext 时对 Python 安装及 sidecar 进程的依赖；在后续 Runtime 阶段支持与 Node.js 宿主同进程集成。
- 通过 OpenAPI 固定快照、contract-sync、Python oracle 和 conformance fixtures 管理跨语言差异，避免 TypeScript 实现与 Python 参考实现发生无声漂移。
- 利用 npm 分包和独立发布能力，让 Protocol、Client、Core、Runtime、Server、CLI 等能力可以按需安装和分阶段发布。

### 面向的用户群体

- 使用 TypeScript/JavaScript 和 Node.js 构建 AI Agent、MCP 服务及上下文工程应用的开发者；
- PowerContext 的 DSH、编辑器扩展、Web tooling 等 Node.js 宿主集成维护者；
- 希望在 Node.js 进程内嵌入 PowerContext 能力，或通过强类型 Client 接入现有 PowerContext Server 的团队；
- 参与 PowerContext 多语言契约、测试和生态建设的社区贡献者。

### 为什么采用独立仓库并在 ob-labs 孵化

- TypeScript 项目使用 Node.js、pnpm、npm 包、独立 CI 和发布节奏，与 Python 项目的 uv/PyPI 工具链和发布周期不同；独立仓库可以保持两端职责及权限边界清晰。
- 相较于 Python 实现，TypeScript 更适合与 Node.js Agent、MCP、编辑器扩展和 Web 工具链同进程集成，并可借助静态类型、Web 标准接口与 npm 分包降低该生态的接入和发布成本。
- 两个仓库只通过受控的 contract-sync 和 oracle/conformance 流程协作，Python 仓库继续作为语义参考，TypeScript 仓库独立管理生成资产、兼容性报告和发布物。
- 项目按里程碑渐进建设：先交付低风险、可独立产生价值的 Protocol + Client，再以 SQLite/Memory FTS 垂直切片验证本地 Runtime，之后决定是否继续扩展完整产品能力。该阶段性路线适合在 ob-labs 中孵化和验证。

### 当前准备情况与建设计划

当前已完成 Phase 0 工程准备，包括 Python 基线锁定、OpenAPI 契约快照、仓库分离与契约同步 ADR、能力清单、RFC 台账、完整对齐定义和风险登记。仓库创建后计划按以下里程碑推进：

1. **M1：Protocol + Client**——发布 TypeScript 协议包和强类型 HTTP Client；
2. **M2：SQLite FTS Runtime**——完成 Memory、FTS 和 PreparedContext 的 Node.js 本地运行闭环；
3. **M3：Domain Runtime**——扩展 Experience、Skill、Handoff、Work Continuity、Review、推理和调度能力；
4. **M4：Full Product**——在一致性与发布质量门通过后，补齐 HTTP、MCP、CLI、可观测性、OceanBase/向量、迁移及完整兼容能力。

每个里程碑都会明确能力范围和兼容等级；未实现或条件可用的能力将显式报告，不会以降级或空结果伪装为完整兼容。

## 项目责任人（GitHub ID）

- Maintainer: knqiufan

## 开源协议

Apache License 2.0，与 PowerContext Python 项目及 OceanBase 社区主流开源协议保持一致。

## 开源项目检查清单

> 检查清单是为了让项目更规范，让社区用户更容易使用。应该在项目创建后，尽快补充清单中的信息。

- [x] 包含 README.md
- [x] 工程类项目包含 CONTRIBUTING.md。参考 OceanBase 社区 [CONTRIBUTING 文件](https://github.com/oceanbase/.github/blob/main/CONTRIBUTING.md)
- [ ] 包含 CODE_OF_CONDUCT.md（没有此文件将使用社区现有的[行为准则文件](https://github.com/oceanbase/.github/blob/main/CODE_OF_CONDUCT.md)）
- [ ] 工程类项目包含用户安装指导说明（将在 Phase 1 工程骨架和首个可安装包完成后补充）
- [ ] 工程类项目包含用户使用指导说明（将在 M1 Protocol + Client 可用后补充）
- [ ] 工程类代码项目包含构建指导说明（将在 Phase 1 pnpm workspace、构建及 CI 建立后补充）

## 投票截止时间

如果不满足投票条件，此投票将在 2026 年 09 月 06 日截止。

> 满足投票条件是指投票已经成功，例如已有不少于 2/3 的 TOC 成员投票通过；或者投票失败，例如有一半的 TOC 成员反对。

## 投票结果

参考 [创建 powercontext-ts 项目投票结果](一个 pull request 链接)。
