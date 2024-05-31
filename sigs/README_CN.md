# Special Interest Group(SIG)

SIG 的全称是 Special Interest Group，即特别兴趣小组。SIG 必须保持开放透明的原则，通过会议分享、项目开发等活动促进技术交流。欢迎任何新人加入 SIG 并作出贡献。

## 加入一个 SIG
如果你对某个领域的话题感兴趣，可以申请加入或关注对应的 SIG。通常 SIG 都有自己的周期性会议、日常沟通群，你可以先参加相关的活动，然后按照对应 SIG 的规定申请加入。

## 创建新的SIG
如果你有新的想法，当前的SIG列表中没有满足你兴趣的 SIG，你可以提出申请创建新的 SIG。请参考下面的申请流程。

注意：SIG 应遵守 [SIG规则](./governance.md)。

**申请流程**

- 提交PR到 [oceanbase/community](https://github.com/oceanbase/community) 仓库，标题为 "SIG Charter Proposal: <your sig-name>"；
- 增加新的 SIG 目录，复制[SIG模板](./sig-template/)，修改目录名为`community/sigs/sig-<sig-name>`，例如`community/sigs/sig-obdiag`，填写模板内容；
- 填写[投票信息](../votes/README_CN.md)；
- 填写 README 文件和 membership.yml 文件。其中 membership.yml 文件填写 Maintainer 信息，和各个项目中的 Committer 信息；
- 按照 review 意见调整 PR 内容；
- 投票审批通过后，PR 会被 merge，SIG 正式成立。必要时会邀请你参会讨论。

投票通过必须满足以下所有条件：
- 不少于 2/3 TOC 成员审批通过；
- 所有 Maintainer 投票通过。

## 更新SIG信息

SIG 信息变更的内容不同，需要由不同角色的人来审核。

投票通过条件：

**SIG 项目列表变更**
- 不少于 2/3 TOC 成员投票通过。

**SIG Maintainer 成员变更**

需要同时满足：
- 不少于 2/3 TOC 成员投票通过；
- 所有新增 Maintainer 成员投票通过。

**其它**
- 不少于 2/3 Maintainer 通过。

**变更流程**

> 这里说明 SIG 普通信息的变更，membership 变更流程请参考 [membership变更流程](./membership.md)。

- 提交PR到[oceanbase/community](https://github.com/oceanbase/community)仓库，PR 标题 `SIG Update: <your sig-name>"`；
- 并填写[投票信息](../votes/README_CN.md)；
- 投票通过后 PR 会被 merge，变更成功。

## 结束SIG
由于某些原因，SIG没有存在的必要性，可以结束 SIG。

**结束流程**
- 提交 PR 到[oceanbase/community](https://github.com/oceanbase/community)仓库，PR 标题为 "SIG Termination: <your sig-name>"，
- 将 sig 目录放入 `community/sigs/archive-sigs` 目录；
- 不少于  2/3 TOC 审批通过后，PR 会被 merge，SIG 终结。

## sigs 目录文件说明
`sigs` 目录，也就是当前目录，存放所有 SIG 组织，`sig-template` 目录存放创建新的 SIG 时的模板文件，archive-sigs 存放不再活跃的 SIG，其余目录以 `sig-<name>` 命名，记录某个 SIG 的信息。普通的 SIG 最少包含两个文件，README 和 membership.yml文件，分别记录 SIG 的信息，比如兴趣组的目标、交流渠道等，membership.yml 文件记录该组的 Maintainer 和各个仓库的 Committer 信息。
