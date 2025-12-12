# 申请创建 PowerContextMgr 项目

## 项目基本信息

项目名称：PowerContextMgr

### 项目目的

从智能体开发的角度出发，任务由Agents组合完成，其中单体Agent的工作实质上可视为上下文的实现。
上下文工程可以分为三个角度，工具调用，记忆管理以及业务相关内容。
受PowerMem-MCP启发，实际上我们可以把记忆管理通过工具调用的方式交互（而不是通过hardcode，从而把控制和反馈的能力交给大模型，增加灵活性）。

#### 项目用于做什么 
PowerContextMgr，将会开启一个探索。尝试将工具调用和记忆管理整合。
- 在交互层面，将记忆调用的方式从代码调用，转为MCP，从而将决定权交还给大模型。
- 在数据层面，无论工具调用还是记忆查询，实际上都是通过查询额外数据提高准确性。

#### 解决什么问题
这个探索将会基于PowerMem-MCP，PowerMem，和SeekDB出发，改进MCP通讯机制。
- 通过统一改进的MCP协议让大模型在agent任务查询时，决定工具使用和记忆内容的引入。
- 通过改进MCP工作流，为PowerMem-MCP实现多模态支撑，从而实现一种统一的（单Agent，单个查询）数据处理流程。
- 通过SeekDB扮演RAG，实现渐进式加载，解决工具选择困难。

#### 面向的用户群体
通过这样的探索，预期在MCP的基础上实现上下文标准（或者一种上下文处理协议？）从而Agent开发人员可以专注于业务流程开发或Agents编排。
同时，通过引入k8s上的服务网格，负载均衡等能力，面向企业用户实现一个上下文抽象层（中间件）。

## 项目责任人(github id)：
- Maintainer: SamYuan1990

## 开源协议：

> 建议采用 Apache 2.0，如果不采用 Apache 2.0 协议，请注明原因

## 开源项目检查清单

> 检查清单是为了让项目更规范，让社区用户更容易使用。应该在项目创建后，尽快补充清单中的信息。

- [ ] 包含 README.md
- [ ] 工程类项目需要包含 CONTRIBUTING.md。参考 OceanBase 社区 [CONTRIBUTING 文件](https://github.com/oceanbase/.github/blob/main/CONTRIBUTING.md)
- [ ] 包含文件 CODE_OF_CONDUCT.md （没有此文件将使用社区现有的[行为准则文件](https://github.com/oceanbase/.github/blob/main/CODE_OF_CONDUCT.md) ）
- [ ] 工程类项目包含用户安装指导说明（通常在README.md中说明）
- [ ] 工程类项目包含用户使用指导说明（通常在README.md中说明）
- [ ] 工程类项目代码类项目包含编译指导说明（通常在README.md中说明）

## 投票截止时间
如果不满足投票条件，此投票将在 2025 年 12 月 31 日截止。

> 满足投票条件是说投票已经成功，比如已经有不少于 2/3 的 TOC 投票，或者投票失败，比如有一半的 TOC 反对。


## 投票结果
参考 [创建 xxx 项目投票结果](一个 pull request链接)。
