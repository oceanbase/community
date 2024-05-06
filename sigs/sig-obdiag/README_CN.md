# SIG obdiag

## obdiag 简介

OceanBase Diagnostic Tool (obdiag) 是一款专门OceanBase打造的敏捷诊断工具，功能包括诊断信息收集、分析、巡检，可以在 OceanBase 集群不同的部署模式下（OCP，OBD 或用户根据文档手工部署）实现一键执行。

### 项目价值
OceanBase 是原生分布式数据库系统，故障根因分析通常是比较繁琐的，因为涉及的因素可能有很多，如机器环境、配置参数、运行负载等等。专家在排查问题的时候需要获取大量的信息来分析故障，如何高效的获取故障场景下分散在各个节点的信息，挖掘出其中的关联性，帮助用户自助诊断问题便是 obdiag 的价值。

![Project Value](images/value.png)

### 特性

#### 产品特性
obdiag 定位为 OceanBase 敏捷诊断工具。整体使用上备以下的特点：

- 极致轻量：提供rpm 包和 OBD 上部署的模式，均可一键部署安装，rpm 包才不到 30MB 大小。可以选择部署到任意一台能连接到集群各个节点的上，并不局限于 OBServer 节点。
- 简单易用：一条命令搞定安装，一键集群巡检、一键信息收集、一键诊断分析、一键根因分析等功能全部可以通过一条命令搞定，简单易用。
- 完全开源：obdiag 是 Python 代码开发的，源代码100%开源，github 地址仓库：https://github.com/oceanbase/obdiag
- 高度可扩展：obdiag 的一键巡检功能、一键场景化信息收集功能、一键根因分析功能都是插件化的，用户可自行低成本的添加场景来定制化诊断的场景。

![features](images/features.png)

#### 功能特性
obdiag 现有功能包含了对于 OceanBase 日志、SQL Audit 以及 OceanBase 进程堆栈等信息进行的扫描、收集、分析、诊断，可以在 OceanBase 集群不同的部署模式下（OCP，OBD 或用户根据文档手工部署）实现一键诊断执行。
![function features](images/function-features.png)

obdiag的功能如下：
- 一键集群巡检：使用 obdiag check 命令可帮助 OceanBase 数据库集群相关状态巡检，目前支持从系统内核参数、内部表等方式对 OceanBase 的集群进行分析，发现已存在或可能会导致集群出现异常问题的原因分析并提供运维建议。
- 一键诊断分析：使用 obdiag analyze 命令可帮助 OceanBase 数据库相关的诊断信息分析，目前支持对 OceanBase 的日志进行一键分析，找出发生过的错误信息；一键全链路诊断分析，展示全链路诊断树，定位链路慢在何处。
- 一键信息收集：使用 obdiag gather 命令可帮助 OceanBase 数据库相关的诊断信息收集。目前支持基础诊断信息收集和基于场景的诊断信息一键收集。
- 一键根因分析：使用 obdiag rca 命令可帮助 OceanBase 数据库相关的诊断信息分析，目前支持对 OceanBase 的异常场景进行分析，找出可能导致问题的原因。

## 关联的代码仓库

- [obdiag](https://github.com/oceanbase/obdiag)

## 语雀文档
[obdiag 语雀空间](https://oceanbase.yuque.com/org-wiki-obtech-vh7w9r/imzr6c/rhg09211pih0aomx)

## 联系信息

周会信息：每周举行一次线上周会，会议时间初定每周五 16:00-17:00。会议纪要记录到外网语雀文档和 GitHub 中
周会归档：[周会记录](https://oceanbase.yuque.com/org-wiki-obtech-vh7w9r/imzr6c/pa2ny21mpif09xot)

微信群：专用微信群【[SIG] OceanBase 诊断工具兴趣小组】，便于成员随时讨论问题，微信群添加方式，添加微信：obdiagsig，说明加群目的，审核通过后管理员会将加用户加入微信群中。

## 组织架构
> 我们要求成立一个SIG，最少有3个人

成员角色说明完全参照[成员角色说明](../membership.md)，没有变更。

### Maintainer

- 白鳝(xuji755), 南京基石数据
- 汤庆(Teingi), OceanBase
- 傅榕锋(frf12), OceanBase

### Committer

- 王煦焱(wayyoungboy), OceanBase

### Contributor

- 肖兵
- 岳艳涛
- 藏强磊
- 陈海英
- 杜振鹏
- 洪云飞
- 靖永栋
- 邱永刚
- 孙鹏
- 唐素珍
