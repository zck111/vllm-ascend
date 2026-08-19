---
name: accuracy
description: "占位子代理：精度 Agent（暂未开发）。Day0 工作流的精度验收后续由本 Agent 承担。当前阶段不要调用，由主 skill 直接提示【精度 Agent 暂未接入】。"
---

# 精度 Agent（占位）

> ⚠️ **占位声明**：本 Agent 尚未开发，`Day0 推理流程编排` 当前阶段**不会调用**它。

## 规划职责（后续开发接入）

- 对齐 Phase 4 验证的「端到端精度」：先 `enforce_eager` 对齐厂商参考实现输出，再开 ACL Graph 对比 eager。
- 依据 Designer 产出的 Golden 基线描述，做 logits / 输出文本 / 指标级对齐。
- 输出：精度对齐报告（逐层最大误差、基准指标 vs Golden）。

## 计划接入点（占位，勿执行）
1. Designer 输出中包含 Golden 基线 + 精度对齐目标。
2. Tester 产出真实权重门（Stage B）通过证据，作为当前阶段精度口径。
3. 主 skill 在「精度验收」阶段改为调用本 Agent，替换当前提示语。
