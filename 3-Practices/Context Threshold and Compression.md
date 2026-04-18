# Context Threshold and Compression

## Rule

当当前对话接近上下文阈值时，先整理、写回、压缩，再继续推进。

不要等上下文已经明显腐烂后才补救。

## 判断方式

采用双轨判断：

- Codex 负责做近似预警
- Xavier 如果看到更准确的 `/usage` 或平台信号，以平台信号为准

Codex 近似预警时主要看：
- 对话长度是否已经明显膨胀
- 工具输出是否持续堆积
- 当前任务是否出现多分支并行
- 是否开始重复检索、重复解释、或明显偏离主线

## 阈值分层

### 70% 左右：轻压缩

默认动作：
- 在当前对话里输出压缩摘要
- 提炼：当前任务、已确认结论、关键页面或文件、风险、未决问题、下一步
- 把值得长期保存的内容写入 Obsidian
- 至少补一条 `4-Episodic/`；必要时同步更新 `5-Projects/`、`6-Users/`、`2-Knowledge/`、`3-Practices/`

目标：
- 降噪
- 防止结论埋没
- 给后续强压缩预留空间

### 85% 左右或出现 context rot：强压缩

默认动作：
- 生成明确 handoff
- 标出已完成、未完成、风险、下一步
- 在当前对话里只保留最小续接信息
- 默认建议切到新 session

## 分类原则

压缩时不要把所有内容都塞进一个地方：

- 一次具体 session 记录：`4-Episodic/`
- 项目事实和决策：`5-Projects/`
- Xavier 的长期偏好、约束、授权边界：`6-Users/Xavier/`
- 可复用的方法抽象：`2-Knowledge/`
- 行为规则和执行步骤：`3-Practices/` 或 `7-Protocols/`

## Anti-pattern

- 明知上下文已经接近阈值，仍继续堆对话
- 只在聊天里总结，不写回 vault
- 只写一条 episodic，不更新对应 canonical page
- 已经出现 context rot，还不做 handoff
