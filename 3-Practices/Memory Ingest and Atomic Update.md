# Memory Ingest and Atomic Update

## Rule

新信息只有在被正确归档、并且影响到的旧页也一起更新后，才算真正进入系统。

## Ingest 流程

1. 先判断材料值不值得长期保存。
2. 原始资料先进入 `1-Sources/` 或 `8-Inbox/`。
3. 写摘要、要点、关联和自己的判断。
4. 找出受影响的旧页并更新。
5. 如有必要，补一条 episodic 记录。

## Atomic Update Checklist

- 这条信息的 canonical home 是哪里？
- 哪个旧页现在已经过时？
- 哪些术语需要统一？
- 哪些 cross-link 现在应该存在？
- 它会不会改变某条 practice 或 protocol？

## Anti-pattern

- 只新建页面，不更新旧页
- 把对话里提到的重要信息留在对话里，不写回系统
- 把短期波动直接升级为长期画像
