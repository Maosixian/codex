# Session Startup Protocol

## Rule

每次新 session，如果任务不是纯闲聊，就先恢复系统上下文，再动手。

这里的“恢复系统上下文”默认包含：
- 读取启动链路
- 检索相关项目页、用户页、episodic、knowledge、practices
- 判断这次工作是否需要在过程中直接写回 vault

## 默认读取顺序

1. `3-Practices/Session Checklist.md`
2. `CODEX.md`
3. `index.md`
4. `3-Practices/README.md`
5. `7-Protocols/README.md`
6. `6-Users/Xavier/About.md`
7. `6-Users/Xavier/Current State.md`
8. `6-Users/Xavier/Preferences.md`
9. `6-Users/Xavier/Values.md`

## 然后按任务类型检索

### 如果是已有项目
- 查 `5-Projects/`
- 查最近相关的 `4-Episodic/`
- 查项目相关知识页

### 如果是关于 Xavier 本人的长期问题
- 查 `6-Users/Xavier/Goals.md`
- 查 `6-Users/Xavier/Patterns.md`
- 查 `6-Users/Xavier/Growth.md`
- 查 `6-Users/Xavier/Commitments.md`
- 查 `6-Users/Xavier/Strengths.md`
- 谨慎查 `6-Users/Xavier/Blindspots.md`

### 如果是 ingest 新材料
- 查 `8-Inbox/`
- 查相关知识页和项目页
- 再决定如何归档

## 禁止的启动方式

- 只凭当前对话就假装自己全记得
- 不读规则就改写系统
- 不检索旧页就直接建新页
- 把读取、记录、调用 Obsidian 当成只有 Xavier 提醒时才做的动作
