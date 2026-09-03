# 申请创建 seekdb-android 代码仓库

## 项目基本信息

项目名称：seekdb-android

项目目的：

seekdb-android 是 SeekDB（OceanBase 开源的嵌入式向量数据库）的 Android 端 SDK：通过 JNI 将原生引擎 libseekdb.so 封装进 Android 应用，并提供与 Room / SupportSQLite 兼容的数据访问层，让 Android 开发者可以使用熟悉的 Room 注解与 DAO 模式开发基于向量检索的端侧 AI 应用。

在 OceanBase 开源生态中的价值包括：

- 与 **SIG AI**「数据库与 AI 双向赋能」方向一致，将 SeekDB 的端侧向量检索能力带到 Android / 移动端，支撑 RAG、Embedding 存储与检索、语义缓存等 AI 场景端上离线运行。
- 面向 Android 生态：以 Room 兼容层接入，迁移成本低；CI 与兼容性测试遵循 AndroidX / sqlite-android 社区惯例（Room P0 场景 + 兼容矩阵回归）。
- 分发便捷：随 tag 通过 JitPack 直接产出内嵌 libseekdb.so 的 AAR，社区用户开箱即用。
- 附带 Database Inspector 支持模块（seekdb-android-inspection），便于开发者 debug 阶段使用。

仓库地址：<https://github.com/ob-labs/seekdb-android>

代码现状：原型与 Room 兼容性验证已完成，当前托管于 <https://github.com/dengfuping/seekdb-android>，待投票通过后迁移至上述仓库地址。

项目责任人（github id）：

- Maintainer: dengfuping

> 其余 Maintainer / Committer 可在评审过程中补充。

开源协议：Apache 2.0（与 OceanBase 社区主流协议及 seekdb 生态仓库保持一致；建仓迁移时同步将 LICENSE / NOTICE 切换为 Apache-2.0）

## 开源项目检查清单

> 检查清单是为了让项目更规范，让社区用户更容易使用。应该在项目创建后，尽快补充清单中的信息。

- [x] 包含 README.md
- [ ] 工程类项目需要包含 CONTRIBUTING.md。参考 OceanBase 社区 [CONTRIBUTING 文件](https://github.com/oceanbase/.github/blob/main/CONTRIBUTING.md)
- [ ] 包含文件 CODE_OF_CONDUCT.md （没有此文件将使用社区现有的[行为准则文件](https://github.com/oceanbase/.github/blob/main/CODE_OF_CONDUCT.md) ）
- [x] 工程类项目包含用户安装指导说明（通常在README.md中说明）
- [x] 工程类项目包含用户使用指导说明（通常在README.md中说明）
- [x] 工程类项目代码类项目包含编译指导说明（通常在README.md中说明）

## 投票截止时间

如果不满足投票条件，此投票将在 **2026 年 9 月 17 日** 截止。

> 满足投票条件是指投票已经成功（例如已有不少于 2/3 的 TOC 投票通过），或投票失败（例如有一半 TOC 反对）。

## 投票结果

参考 [创建 seekdb-android 项目投票结果](https://github.com/oceanbase/community/pull/87)。
