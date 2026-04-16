# Retrieval Model

## 核心思想

`codex` 不把单次对话上下文当作唯一记忆，而把 vault 当作主记忆载体。

这个模型接近 Karpathy 的 LLM Wiki 思路：
- `1-Sources/` 是原始来源
- `2-9` 层是可读可写的 wiki
- `CODEX.md` 是 schema

如果 schema 不稳定，wiki 会腐烂。
如果 wiki 不被检索，记忆就等于不存在。

## 检索默认顺序

### 1. Schema
先读系统规则，避免一上来乱写。

### 2. User model
如果任务和 Xavier 的偏好、目标、成长有关，先看 `6-Users/Xavier/`。

### 3. Project memory
如果任务属于已有项目，先看 `5-Projects/`。

### 4. Episodic history
如果要恢复上下文、接着上次做，先看最近和相关的 `4-Episodic/`。

### 5. Knowledge and practices
如果要回答方法、架构、流程问题，先看 `2-Knowledge/` 和 `3-Practices/`。

### 6. Sources and inbox
如果判断需要原始材料或刚进来的材料，再看 `1-Sources/` 和 `8-Inbox/`。

## 创建新页面前的默认问题

1. 这个概念已经有没有 canonical page？
2. 我是不是应该更新旧页，而不是新建一页？
3. 这条信息属于项目、用户、方法、历史，还是原始资料？
4. 它是不是只应该留在当前 session，而不值得长期保存？

## 成功标准

检索系统有效时：
- 新 session 不用从头猜
- 相似问题能复用旧答案
- 旧认知能随着新信息更新
- 页面数量增加，但噪音不失控
