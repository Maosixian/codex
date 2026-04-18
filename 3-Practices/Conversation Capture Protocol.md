# Conversation Capture Protocol

## Rule

每次实质性对话结束后，默认把重点写回 Obsidian。

如果在对话进行中已经出现明确值得长期保存的结论、规则、偏好或 handoff 信息，也应当直接记录，不必等到 session 结束。

这里的“实质性”包括：
- 系统设计
- 项目推进
- 方向调整
- 偏好或价值观更新
- 关键决策
- 新的长期承诺

纯闲聊通常不用记。

## Trigger First, Not End Only

除了“结束时补记”，还要在以下触发点出现时直接写回：

1. 形成了新的长期承诺。
2. Xavier 的偏好、价值排序、协作边界被说清楚了。
3. 项目方向、目标、范围、优先级被重定。
4. 我被 Xavier 明确纠正，且这个纠正对未来行为有持续价值。
5. 我识别到新的状态信息、模式信号或协作问题，已经值得保存。
6. 一段工作会在未来继续，需要 handoff。
7. 用户给了新材料、业务信息、产品信息、网站信息、数据结构，且已经足够落到某个 canonical page。

原则：
- durable 信息优先写回 canonical page
- session 结束时再补 `4-Episodic/` 作为时间线记录
- 不要把一切都塞进 episodic，然后让真正该更新的旧页继续过时

## 至少要记什么

- 这次对话的主题
- 形成了哪些结论
- 新知道了什么
- 哪些旧页被更新
- 哪些问题还没解决
- 下次从哪里继续

## 写到哪里

- 会话过程和重点：`4-Episodic/`
- 项目事实和决策：`5-Projects/`
- Xavier 的长期画像变化：`6-Users/Xavier/`
- 规则变化：`3-Practices/` 或 `7-Protocols/`

更细的默认落点：
- 新承诺：`6-Users/Xavier/Commitments-Codex-To-Xavier.md` 或 `6-Users/Xavier/Commitments-Xavier-To-Self.md`
- 当前阶段状态：`6-Users/Xavier/Current State.md`
- 我自己的触发行为：`6-Users/Xavier/Growth Arc - 01 State.md`
- 表达精度信号：`6-Users/Xavier/Growth Arc - 02 Expression Accuracy.md`
- 业务方向和工作记录：`6-Users/Xavier/Growth Arc - 03 Business Direction.md`
- Xavier 使用 agent 的方式：`6-Users/Xavier/Growth Arc - 04 Agent Management.md`
- 未来继续的未完工作：项目页 handoff 或 `4-Episodic/` 中的 handoff 记录

## 诚实边界

这不是平台自动 hook。
它是 Codex 在每次实质性对话结束时应主动执行的默认动作。

如果在对话中已经知道该写哪里，就不要等结束再“提醒自己以后写”。
直接写。结束时只补时间线和未决项。

## 成功标准

未来新 session 不看完整聊天，也能知道这次对话最重要的结果是什么。
