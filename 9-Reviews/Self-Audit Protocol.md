# Self-Audit Protocol

## Purpose

这个协议解决的不是“规则缺不缺”，而是“规则有没有真的在运行”。

如果 Codex 只会写 practices，却不定期检查 capture、commitments、Xavier 模型和系统漂移，那系统就会变成装饰品。

## Cadence

- 默认每 `2` 天检查一次
- 触发点写在 `3-Practices/Session Checklist.md` 和 `3-Practices/Session Startup Protocol.md`
- 如果最近没有 `*-self-audit*.md`，视为已过期

## Trigger

每次新 session 开始时：

1. 找 `4-Episodic/` 最新的 `*-self-audit*.md`
2. 如果没有，或距离今天已满 `2` 天，先做这份自审
3. 如果用户问题紧急，可以先回应，但这一轮必须补做，并在自审里写明原因

## Audit Checklist

### 1. Capture Freshness

- 最近 `2` 天的实质性 session 有没有留下 `4-Episodic/` 记录
- 如果漏了，至少补最关键的一条

### 2. Xavier Model Freshness

- `6-Users/Xavier/About.md` 有没有已经知道但还没写进去的信息
- `6-Users/Xavier/Current State.md` 现在的阶段描述还准不准
- `6-Users/Xavier/Commitments-*.md` 有没有该更新状态的项

### 3. Growth Activity

- `Growth Arc - 01 State` 最近有没有该记的信号
- `Growth Arc - 03 Business Direction` 最近有没有该记的工作/方向变化
- 其他 arc 有没有明显新证据

### 4. Commitments Review

- `Commitments-Codex-To-Xavier.md` 有没有 overdue、完成、失效或需要改写的项
- `Commitments-Xavier-To-Self.md` 有没有需要提醒的项

### 5. Drift And Contradictions

- 最近新信息有没有让旧页过时但还没更新
- 有没有只新建没回写旧页
- 有没有明显孤立页面或失去用途的页面

## Output

每次自审都产出一条：

`4-Episodic/YYYY-MM-DD-self-audit.md`

建议格式：

```md
# Self-Audit YYYY-MM-DD

**Last audit**: YYYY-MM-DD 或 none

## 1. Capture freshness
- ...

## 2. Xavier model freshness
- ...

## 3. Growth activity
- ...

## 4. Commitments
- ...

## 5. Drift and contradictions
- ...

## Next audit due
- YYYY-MM-DD
```

## Anti-Patterns

- 把自审做成形式主义，只写“都很好”
- 自审发现问题，却不补救
- 明知过期，还继续假装系统健康

## Success Condition

- `4-Episodic/` 大体每 `2` 天有一次自审
- Xavier 相关页面会在用户没提醒时也被更新
- commitments 和 growth 不会长期停在 day-0
