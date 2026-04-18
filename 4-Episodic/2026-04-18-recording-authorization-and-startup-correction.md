# 2026-04-18 — recording authorization and startup correction

## Session
- 日期：2026-04-18
- 主题：修正新 session 未先读 vault 的问题，并明确记录/删除的授权边界
- 相关项目：[[../5-Projects/Codex System]]

## State
- 当前目标：让 `codex` 的长期记忆系统从“有规则”进一步变成“更稳定执行”
- 当前阶段：在真实对话中校正启动流程与记录动作
- 当前卡点：平台层面仍然没有真正的强制 hook，执行仍依赖 Codex 主动遵守协议
- 当前优先级：先保证新 session 读取和会话中途记录更稳定
- 当前限制：仍然只能修改 `codex`，不能动其他 vault，也不能动 `obsidian-auto-sync`

## Did
- Xavier 指出：新的 session 没有先按规则读取 Obsidian vault
- Codex 补读了 `CODEX.md`、startup、user pages，并恢复到 vault-first 流程
- 检索并确认：关于 conversation capture、session handoff、memory ingest 的页面已经存在
- Xavier 明确授权：今后记录、补记、更新 Obsidian 中相关内容不需要逐次征求同意
- 同时明确边界：删除 vault 内容必须先得到 Xavier 的明确授权
- 把这条授权边界写入协议、承诺和历史页面
- Xavier 进一步明确：不只是新 session，旧 session 在推进过程中也应默认主动读取、调用、记录 Obsidian
- 把这条“默认而非提醒驱动”的要求写入 schema、startup、execution 和 Xavier 页面

## Learned
- 现在的主要问题不是分类结构不够，而是记录和检索动作是否足够稳定地发生
- Xavier 希望“发现值得记录的内容就直接记录”，而不是等提醒或只在 session 结束时才处理
- 对跨 session 连续性来说，写入授权和删除授权必须明确分开
- 要想让系统真的可用，Obsidian 的读取、调用、记录必须变成默认行为，而不是用户提醒后的补救动作

## Updated
- `7-Protocols/Memory Write Policy.md`
- `3-Practices/Conversation Capture Protocol.md`
- `3-Practices/Session Startup Protocol.md`
- `3-Practices/Execution Workflow.md`
- `6-Users/Xavier/Commitments.md`
- `6-Users/Xavier/Current State.md`
- `6-Users/Xavier/History.md`
- `CODEX.md`
- `4-Episodic/2026-04-18-recording-authorization-and-startup-correction.md`

## Verified
- 已把“记录默认可直接执行、删除必须先授权”的边界写入 `7-Protocols/Memory Write Policy.md`
- 已把“对话进行中出现值得长期保存的内容时，也应直接记录”写入 `3-Practices/Conversation Capture Protocol.md`
- 已把本次授权节点写入 `6-Users/Xavier/History.md` 和 `6-Users/Xavier/Commitments.md`

## Open
- 平台级自动读取/自动写回依然不是强制 hook

## Next
- 继续在真实对话中执行“发现值得记录的内容就中途写回”的默认动作
- 在实际使用中检查：`70%` 和 `85%` 阈值是否需要进一步调优
