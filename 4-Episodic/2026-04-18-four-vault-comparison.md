# 2026-04-18 — four vault comparison

## Session
- 日期：2026-04-18
- 主题：比较 `claude`、`free-code`、`hermes`、`codex` 四个 vault，并继续把综合版收束进 `codex`
- 相关项目：[[../5-Projects/Codex System]]

## State
- 当前目标：明确四个 vault 的差异，并让 `codex` 更接近唯一主系统
- 当前阶段：从“已具备骨架”推进到“更像真正运行中的综合版”
- 当前卡点：平台本身没有保证每个新对话都自动读取/自动写回 vault 的强制 hook
- 当前优先级：只修改 `codex`，吸收其他 vault 的优点，不碰其他 vault
- 当前限制：不能修改其他 vault，也不能修改 `obsidian-auto-sync`

## Did
- 重新比较了四个 vault 的目标、入口和分层
- 确认 `claude` 更强在长期伙伴与 Xavier 模型
- 确认 `free-code` 更强在工程执行与 anti-drift 分层
- 确认 `hermes` 更强在状态校准、价值排序和战友式边界
- 在 `codex` 中新增了状态校准与会话记录协议

## Learned
- `codex` 已经是最适合继续演化为综合版主 vault 的底子
- 真正的难点不是结构设计，而是如何把“读 vault / 记对话”变成稳定默认动作
- 在不动平台和其他仓库的前提下，最强可实现方案是把这些动作写进 `codex` 的启动与记录协议里

## Updated
- `CODEX.md`
- `index.md`
- `3-Practices/State Calibration.md`
- `3-Practices/Conversation Capture Protocol.md`
- `3-Practices/Session Checklist.md`
- `3-Practices/Session Startup Protocol.md`
- `3-Practices/Session Logging and Handoff.md`
- `4-Episodic/Episodic Entry Template.md`
- `6-Users/Xavier/Current State.md`
- `6-Users/Xavier/About.md`
- `6-Users/Xavier/Goals.md`
- `6-Users/Xavier/History.md`

## Verified
- 只修改了 `codex`
- 新增协议已经挂进 `CODEX.md`、`index.md` 和 `3-Practices/README.md`

## Open
- 平台级“每次新对话自动执行”仍然不是强制 hook
- 还没有做周期性 review 和 lint 的真实样本

## Next
- 继续把后续实质性对话按新协议写回 `4-Episodic/`
- 在实际使用中检验：新 session 是否真的先检索、先校准、再行动
