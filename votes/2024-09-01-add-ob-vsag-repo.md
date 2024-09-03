# 申请添加 ob-vsag 代码仓库

## 项目基本信息

项目名称：ob-vsag

项目目的：给 oceanbase 增加基于开源向量检索库vsag封装的OceanBase向量检索插件

ob-vsag 是 [OceanBase](https://github.com/oceanbase/oceanbase) 团队基于蚂蚁集团 [vsag](https://github.com/alipay/vsag) 构建的。vsag 是一个用 C++ 编写的向量索引库，专门用于相似性搜索。该索引算法库提供了基于向量维度和数据规模生成参数的方法，使用户能够搜索不同规模的向量数据集，并且开发人员无需了解算法的具体原理即可进行集成和使用。

- 在 vsag 提供的基础向量检索能力基础适配 Oceanbase 内核向量索引接口
- 支持在 OceanBase 数据库上运行和使用 vsag 提供的相关向量检索能力

项目责任人（github id）：
- PMC：akaError
- PMC：caifeizhi
- committer：Carrot-77
- committer: a1iive

开源协议：Apache 2.0

## 开源项目检查清单

> 检查清单是为了让项目更规范，让社区用户更容易使用。应该在项目创建后，尽快补充清单中的信息。

- [Y] 包含 README.md
- [N] 工程类项目需要包含 CONTRIBUTING.md。参考 OceanBase 社区 [CONTRIBUTING 文件](https://github.com/oceanbase/.github/blob/main/CONTRIBUTING.md)
- [Y] 包含文件 CODE_OF_CONDUCT.md （没有此文件将使用社区现有的[行为准则文件](https://github.com/oceanbase/.github/blob/main/CODE_OF_CONDUCT.md) ）
- [Y] 工程类项目包含用户安装指导说明（通常在README.md中说明）
- [Y] 工程类项目包含用户使用指导说明（通常在README.md中说明）
- [Y] 工程类项目代码类项目包含编译指导说明（通常在README.md中说明）

## 投票截止时间

如果不满足投票条件，此投票将在 2024 年 9 月 15 日截止。

> 满足投票条件是说投票已经成功，比如已经有不少于 2/3 的 TOC 投票，或者投票失败，比如有一半的 TOC 反对。

## 投票结果

参考 [申请添加 ob-vsag 代码仓库投票结果](https://github.com/oceanbase/community/pull/16)。
