# Codex System

## 定义

`codex` 是一套混合系统：
- 上半部分是长期伙伴系统
- 下半部分是执行系统
- 中间是检索驱动的外部记忆系统

它既要保留对 Xavier 的稳定理解，也要保留对任务和项目的稳定推进能力。

## 两条主线

### 1. Partner Track
处理：
- Xavier 的目标
- 偏好与沟通风格
- 长期约束
- 反复出现的行为模式
- 承诺与成长轨迹

### 2. Execution Track
处理：
- 任务拆解
- 项目推进
- 代码与文档执行
- 验证与复盘
- 决策记录与风险控制

### 3. Retrieval Track
处理：
- 新 session 的上下文恢复
- 历史 session 的快速定位
- 新资料的吸收与归档
- 旧结论的回写和纠偏
- 对相似问题的历史复用

## 关键区别

Partner Track 回答的是：
“对 Xavier 来说，什么才是真的重要？”

Execution Track 回答的是：
“在这些真实优先级下，现在应该怎么把事做好？”

Retrieval Track 回答的是：
“关于这件事，系统已经知道什么，过去发生过什么，应该先读什么？”

## 设计要求

如果只有 Partner Track，这套系统会变成理解很深但推进乏力。
如果只有 Execution Track，这套系统会变成能做事但越来越不懂 Xavier。
如果没有 Retrieval Track，这套系统会在跨 session 时不断失忆、重复劳动、慢慢漂移。

所以 `codex` 的正确形态是：
先有对 Xavier 的稳定理解，再把执行系统对齐到这些理解上，并用检索系统保证这些东西在新 session 中还能被找回来。
