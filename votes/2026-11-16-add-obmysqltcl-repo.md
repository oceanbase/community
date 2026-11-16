# 申请创建 obmysqltcl 项目

## 项目基本信息

项目名称：obmysqltcl

项目目的：为 Tcl 应用提供连接 OceanBase MySQL 租户的绑定。绑定基于 mysqltcl，使用单独安装的 OceanBase Connector/C（`libobclient`，共享库名为 `libobclnt.so`）。独立仓库将集中维护绑定源码和构建文档，方便 HammerDB 维护者 fork 仓库、制作 BAWT 所需的 ZIP 源码包，并独立构建和验证 HammerDB 安装包。背景见 [HammerDB PR #949 的评审意见](https://github.com/TPC-Council/HammerDB/pull/949#pullrequestreview-5802087432)。

首期内容：

- 迁入[现有绑定](https://github.com/oceanbase/HammerDB/tree/7647f750c93bb220aa9b791bcf5a5b987bf5aa5a/Build/obmysqltcl)的源码、构建脚本、Tcl 包索引及版权和许可声明。
- 提供 Linux 下使用 Tcl 9 和 OceanBase Connector/C 的构建、安装和使用说明。Windows 支持待取得适用的客户端库并完成绑定构建和运行验证后再评估。

拟创建仓库：https://github.com/oceanbase/obmysqltcl

项目责任人（GitHub ID）：

- Maintainer: [jackysp](https://github.com/jackysp)

开源协议：项目基于 mysqltcl 3.052.1 派生，沿用其原有许可，并保留随构建产物分发的 Tcl stubs 的独立许可声明。详见现有 [COPYING](https://github.com/oceanbase/HammerDB/blob/7647f750c93bb220aa9b791bcf5a5b987bf5aa5a/Build/obmysqltcl/COPYING) 和 [NOTICE](https://github.com/oceanbase/HammerDB/blob/7647f750c93bb220aa9b791bcf5a5b987bf5aa5a/Build/obmysqltcl/NOTICE)。

## 开源项目检查清单

> 项目创建后，尽快补充以下信息。

- [ ] 包含 README.md
- [ ] 包含 CONTRIBUTING.md，参考 OceanBase 社区 [CONTRIBUTING 文件](https://github.com/oceanbase/.github/blob/main/CONTRIBUTING.md)
- [ ] 包含 CODE_OF_CONDUCT.md。未提供时使用社区现有的[行为准则文件](https://github.com/oceanbase/.github/blob/main/CODE_OF_CONDUCT.md)
- [ ] 包含安装说明
- [ ] 包含使用说明和示例
- [ ] 包含构建说明

## 投票截止时间

如果不满足投票条件，此投票将在 **2026 年 11 月 30 日** 截止。

> 投票通过需不少于 2/3 的 TOC 成员同意，具体规则见[投票说明](./README_CN.md)。

## 投票结果

待 TOC 投票，投票讨论见本申请 PR。
