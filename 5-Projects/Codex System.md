# Codex System Project

## About

这是 Xavier 与 Codex 的长期协作系统工程。

目标不是做一个漂亮的 vault，而是做一个长期能用的外部脑：
- 能理解 Xavier
- 能推进执行
- 能在新 session 恢复上下文
- 能持续积累长期记忆

## Current State

- 第一版混合骨架已建立
- 已吸收 `claude` 的伙伴系统思路
- 已吸收 `free-code` 的执行系统思路
- 已加入 LLM Wiki 式 schema + wiki + source 的记忆框架
- 还没有大规模迁移旧 vault 的高价值内容

## Decisions

- `codex` 采用 9 层结构，沿用 `free-code` 的分层思路
- `6-Users/Xavier/` 承载长期伙伴画像，沿用 `claude` 的人物建模思路
- 新 session 默认先读 schema，再检索 Obsidian
- 重要 session 默认留下可续接记录
- 不承诺字面上的无限上下文，改为可持续增长的外部长期记忆
- 上下文接近 `70%` 时默认进入整理与轻压缩；接近 `85%` 或明显出现 context rot 时升级为 handoff 与建议切新 session

## Risks

- 如果后续不持续回写，系统会再次退化成“看起来完整但实际不更新”
- 如果迁移旧内容过多过快，容易把噪音也带进来
- 如果 session 不做 handoff，跨 session 的连续性会弱化
- 如果阈值管理只停留在口头约定，不挂到知识页和实践页里，后续仍然会漂移

## Related

- [[../2-Knowledge/Context Threshold Model]]
- [[../3-Practices/Context Threshold and Compression]]

## Commands

- 无固定命令
- 主要动作是阅读、检索、回写、交叉链接和定期整理

## Handoff

- 下次继续前先读：`CODEX.md`、`index.md`、本页、最近的 `4-Episodic/`
- 当前最重要的下一步：从 `claude` 和 `free-code` 精选迁移高价值页面，而不是全量复制
- 已验证：核心结构和关键入口文件已存在
- 未验证：实际长期使用中的检索效率和维护负担
