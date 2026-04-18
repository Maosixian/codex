# 2026-04-19 — growth partner upgrade

## Session
- 日期：2026-04-19
- 主题：吸收 Claude vault 在增长伙伴协作上的关键执行机制，并按 Codex 结构落地
- 相关项目：[[../5-Projects/Codex System]]

## Read

本轮直接读了这些 Claude vault 文件：
- `claude/CLAUDE.md`
- `claude/3-Practices/Commitment Ledger/claude-to-xavier.md`
- `claude/3-Practices/Challenge Protocol.md`
- `claude/3-Practices/Self-Audit Cadence.md`
- `claude/3-Practices/Conversation Capture Protocol.md`
- `claude/3-Practices/Memory Atomic Update.md`
- `claude/3-Practices/Ingesting User Materials.md`
- `claude/3-Practices/Session Handoff Protocol.md`
- `claude/3-Practices/State Calibration.md`
- `claude/6-Growth/arcs/01-state.md`
- `claude/6-Growth/arcs/02-expression-accuracy.md`
- `claude/6-Growth/arcs/03-business-direction.md`
- `claude/6-Growth/arcs/04-agent-management.md`

对照读取了这些 Codex 文件：
- `CODEX.md`
- `index.md`
- `3-Practices/Session Checklist.md`
- `3-Practices/Session Startup Protocol.md`
- `3-Practices/Partnering Workflow.md`
- `3-Practices/Conversation Capture Protocol.md`
- `3-Practices/Execution Workflow.md`
- `3-Practices/Memory Ingest and Atomic Update.md`
- `3-Practices/Session Logging and Handoff.md`
- `7-Protocols/Decision and Challenge Boundary.md`
- `9-Reviews/README.md`
- `6-Users/Xavier/Commitments.md`
- `6-Users/Xavier/Growth.md`

## Judgment

Codex 真缺的不是“再多一点原则”，而是把原则变成触发器和检查点。

确认存在的缺口：
- 缺 `Self-Audit` 机械触发，导致系统健康没人检查
- `不吝惜` 在 Codex 中存在，但还不是最硬的 mandate
- 缺 `Challenge Protocol`，只有边界，没有触发条件和说法
- commitments 是单页混写，启动时不会稳定检查
- growth 只有静态总页，没有动态跟踪结构
- capture 虽然写了“结束后记录”，但对“中途何时必须写回”还不够机械

确认不该照搬的地方：
- 不复制 Claude 的 7 层目录和 `6-Growth/` 位置
- 不把所有记录都推向同一种文件
- 不把 Codex 变成 Claude 的翻版；保留 Codex 的 `6-Users/` 和 `9-Reviews/` 分工

## Did

- 在 `CODEX.md` 提升了“不要把重要真话磨平”的 mandate，并加入 `audit the system` 和 `capture on trigger`
- 新增 `3-Practices/Challenge Protocol.md`
- 新增 `9-Reviews/Self-Audit Protocol.md`
- 把 `Self-Audit` 触发写入 `Session Checklist` 和 `Session Startup Protocol`
- 强化 `Conversation Capture Protocol`，明确中途写回触发点和 canonical 落点
- 更新 `Execution Workflow`，要求 durable 信息出现时直接写回
- 拆分 commitments：
  - `6-Users/Xavier/Commitments-Codex-To-Xavier.md`
  - `6-Users/Xavier/Commitments-Xavier-To-Self.md`
  - `6-Users/Xavier/Commitments.md` 改为总入口
- 将 `Growth.md` 改为入口，并新增 4 条 dynamic arcs：
  - `Growth Arc - 01 State`
  - `Growth Arc - 02 Expression Accuracy`
  - `Growth Arc - 03 Business Direction`
  - `Growth Arc - 04 Agent Management`
- 更新 `index.md`、`3-Practices/README.md`、`9-Reviews/README.md`
- 更新 `6-Users/Xavier/History.md`
- 写入今日首条 `self-audit`

## Not Done

- 没把旧 episodic 全面回填成更细的 growth arc 历史
  - 原因：这轮优先目标是先把运行机制补上，不先做大规模历史重构
- 没新增专门的 “capture triggers” 独立文件
  - 原因：当前更适合把触发逻辑直接压进 `Conversation Capture Protocol` 和 `Execution Workflow`
- 没复制 Claude 的 `6-Growth/` 目录结构
  - 原因：Codex 已有 `6-Users/` 作为用户理解层，继续沿用更一致

## Intentional Differences

- `Self-Audit` 放在 `9-Reviews/`，不是 `3-Practices/`
  - 这是有意保留。它既是协议，也是系统健康检查，更适合 review 层
- Growth arcs 放在 `6-Users/Xavier/`，不是单独做一个 `6-Growth/`
  - 这是有意保留。Codex 的人物理解层已经在这里，拆出去会打散检索路径
- challenge 的“提醒一次就停”仍保留在 Codex 的 boundary 思路里
  - 这是有意保留，不是未解决问题

## Open

- 新增的自审和 capture triggers 还需要在真实 session 中验证是否能持续运行
- 未来可能还需要补 weekly / monthly review 节奏，但这不是当前第一优先级

## Next

- 在后续真实对话中检查：中途写回是否真的发生，而不是重新退化成“最后补总结”
- 到 `2026-04-21` 前后执行下一次 self-audit，验证新机制有没有开始起作用
