# 算法训练入口

> 本目录把学习路线、具体 LeetCode 题目、训练记录和复测连接起来。  
> 算法主语言固定为 Python。

## 文件

- [`problem-bank.md`](./problem-bank.md)：60 题自有题单、官方链接、优先级、四周使用顺序和混合模拟池；
- [`attempt-ledger.md`](./attempt-ledger.md)：每次训练的原始记录、主要错因和 D+1/D+3/D+7；
- 上级 [`../04-algorithm-training-system.md`](../04-algorithm-training-system.md)：训练方法、指标和 AI 使用边界；
- [`../schedule/progress-ledger.md`](../schedule/progress-ledger.md)：跨领域总账，只记录汇总状态和到期复测。

## 使用顺序

```text
查看总账 DUE
→ 从 problem-bank 选择当天题目
→ 首轮隐藏专题并独立尝试
→ 在 attempt-ledger 记录原始过程
→ 验收代码、边界与解释
→ 更新 D+1/D+3/D+7
→ 把周指标同步到 progress-ledger
```

## 当前第一动作

执行 `W0-D1-ALG-01`：

- `SW-03`：209. 长度最小的子数组；
- `BS-04`：33. 搜索旋转排序数组；
- `ST-03`：739. 每日温度。

每题 8 分钟，`/exam` A0，只做无标签分析。若最近 30 天看过题解或完整记得代码，按题单中的替换规则换题。
