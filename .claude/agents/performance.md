---
name: performance
description: "占位子代理：性能 Agent（暂未开发）。Day0 工作流的性能验收后续由本 Agent 承担。当前阶段不要调用，由主 skill 直接提示【性能 Agent 暂未接入】。"
---

# 性能 Agent（占位）

> ⚠️ **占位声明**：本 Agent 尚未开发，`Day0 推理流程编排` 当前阶段**不会调用**它。

## 规划职责（后续开发接入）

- 在 Tester 拉起服务后，跑 `benchmarks/**`，测量 throughput、latency、TTFT/TPOT。
- 若定位到算子性能瓶颈，按架构图约定**workflow 到此结束，转交算子团队优化**（不阻塞 Day0 功能开箱）。
- 输出：性能报告（吞吐 / latency / TTFT / TPOT + 命令与环境 + 硬件代次）。

## 计划接入点（占位，勿执行）
1. Tester 产出服务成功 + 基准吞吐数据，供性能 Agent 对比/深化。
2. 主 skill 在「性能验收」阶段改为调用本 Agent，替换当前提示语。
