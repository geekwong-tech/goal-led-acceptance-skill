# 围绕目标逐步验收

[English](README.md) | 简体中文

这是一个可复用的 agent skill：围绕核心目标，带用户逐步验收实际交付物，每次确认一个判断。适用于网站、手册、报告及其他成果。它不能替代实施审查、用户判断或效果测量。

## 使用方法

将 `skills/goal-led-acceptance` 整个目录复制到 agent 支持的技能目录（Codex 为 `~/.codex/skills/`），然后调用：

```text
请使用 $goal-led-acceptance 的完整中文版，围绕核心目标带我验收这份交付物。一次只走一个验收单元，等我确认再继续。
```

如果当前上下文还没有目标和权威资料位置，请补充这些信息。agent 应先复用已有决策和证据，查看实际成果，区分工具检查、人工验收与实验验证，并让结论不超出证据的支持范围。你可以要求加快、跳过某环节或批量验收。

本 skill 不授予发布或关闭任务的权限，不保证业务效果，也不要求特定工具或其他 skill。设计验收、上线就绪和实际效果仍是不同的判断。

## 文件与维护

- [完整中文技能指引](skills/goal-led-acceptance/SKILL.zh-CN.md)
- [中文虚构示例](skills/goal-led-acceptance/references/example.zh-CN.md)
- [行为验证记录（英文）](tests/validation.md)
- [中文版本验证记录](tests/chinese-validation.md)

本仓库是唯一维护源。安装副本属于分发版本，应从本仓库更新。示例与测试材料均为虚构，不含客户或私有项目数据。

默认发现入口仍是 `SKILL.md`；它提供中文版导航。中文版本与英文版本遵循相同规则，不是另一套流程。安装时保留整个目录，以便导航与参考链接正常工作。

采用 MIT 许可证，见 [LICENSE](LICENSE)。
