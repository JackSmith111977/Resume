# 算法训练入口

> 当前基线：历史上做过约 200 题，但停练约两个月；本轮按未掌握从头重建。  
> 算法主语言固定为 Python，默认使用 ACM 输入输出模式。

## 文件

- [`AGENTS.md`](./AGENTS.md)：算法教学强制规则；每次讲题必须先展示自包含题目卡，并明确 ACM 输入输出，再进入苏格拉底式提问；
- [`problem-bank.md`](./problem-bank.md)：按学习依赖排列的自有 LeetCode 题单、官方链接、角色和五周顺序；
- [`reset-roadmap-2026-08-04.md`](./reset-roadmap-2026-08-04.md)：本轮从零重建路线，覆盖原日历中过早的无标签诊断；
- [`attempt-ledger.md`](./attempt-ledger.md)：每次训练的原始记录、主要错因和 D+1/D+3/D+7；
- 上级 [`../04-algorithm-training-system.md`](../04-algorithm-training-system.md)：训练方法、指标和 AI 使用边界；
- [`../schedule/progress-ledger.md`](../schedule/progress-ledger.md)：跨领域总账，只记录汇总状态和到期复测。

处理本目录中的任何算法教学或复测任务前，必须先读取本目录 `AGENTS.md` 和上级 `../AGENTS.md`。

## 当前策略

```text
新主题：讲解 + 手算 + ACM 引导实现
→ 同类第二题：限时独立尝试
→ D+1 / D+3 / D+7
→ 至少 12 道题通过 D+7
→ 再进入无标签混合模拟
```

- 前两周以 `/tutor` A1/A2 为主；
- 不再直接把中等题作为 A0 基线考试；
- 历史做过的题也必须重新通过解释、实现和复测；
- 题量不是当前目标，能说清状态和独立修改才算恢复；
- LeetCode 作为题源，默认转换为明确的 ACM 标准输入输出；
- 除非用户明确要求，不使用 `class Solution` 函数补全格式。

## 当前第一动作

执行 `W0-D1-ALG-RESET-01`：

- 题目：[`P0-01` 两数之和](https://leetcode.cn/problems/two-sum/)；
- 模式：`/tutor` A1，卡住后最多 A2；
- 开始时先按 [`AGENTS.md`](./AGENTS.md) 展示完整题目卡与 ACM 输入输出；
- 先回答最直接的暴力方案和复杂度；
- 再手算哈希表每一步保存的内容；
- 最后用 Python 从空文件实现并写 3 个测试。

今天不做 209、33、739 的三题无标签诊断。
