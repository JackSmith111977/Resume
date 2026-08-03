# 人机协作任务模板

> 每次开始 S/M/L 任务时复制一份。AI 可以预填，但目标、事实、验收和状态升级由用户最终确认。

## 1. Task Contract

```text
日期：

流水线：能力 / 项目 / 求职 / 反馈
主题：
任务：
任务尺寸：S / M / L

协作模式：/tutor /exam /interview /review /build /archive
最高援助：A0 / A1 / A2 / A3 / A4

当前任务状态：BACKLOG / READY / DOING / REVIEW / VERIFIED
当前能力状态：TODO / LEARNING / CAN_EXPLAIN / CAN_IMPLEMENT / USED_IN_PROJECT / INTERVIEW_READY

独立尝试时间：
本次可见产物：
完成判定：
```

## 2. Human First

```text
我对问题的理解：

它解决什么问题：

我的预测或初始方案：

已知约束：

我已经尝试：

当前卡点：
```

算法任务追加：

```text
题目信号：
暴力方案：
暴力瓶颈：
候选模式：
状态：
不变量：
边界：
复杂度：
```

项目任务追加：

```text
用户问题：
输入和输出：
非功能约束：
最小范围：
明确不做：
验收测试：
```

简历任务追加：

```text
业务/技术背景：
我个人负责：
关键动作：
使用的机制：
结果：
证据来源：
保密边界：
仍未确认：
```

## 3. AI Assistance Log

```text
AI 诊断的错因：
- KNOWLEDGE_MISSING / PATTERN_UNKNOWN / RETRIEVAL_FAILED
- STATE_UNCLEAR / IMPLEMENTATION_FAILED / BOUNDARY_FAILED
- EXPRESSION_WEAK / SOLUTION_MEMORY / OTHER

AI 使用的援助等级：

AI 提供：

我采纳：

我拒绝：

需要事实或测试核验：
```

## 4. Verification

### 通用验收

- [ ] Explain：不看资料讲清楚
- [ ] Predict：能预测新输入、异常或边界
- [ ] Modify：条件变化后仍能解决或修改
- [ ] Test：有测试、反例、演示或模拟证据

### AI 代码额外验收

- [ ] 看过完整 Diff
- [ ] 能解释关键数据流和分支
- [ ] 能删除并补回一小段核心逻辑
- [ ] 能修改一个小需求
- [ ] 能判断至少一个失败测试
- [ ] 检查未擅自扩大项目范围

### 简历额外验收

- [ ] 事实由本人确认
- [ ] 团队成果与个人贡献已分离
- [ ] 指标有来源或已删除
- [ ] 技术结论准确
- [ ] 能回答对抗性追问

## 5. Result

```text
本次产物：

人独立完成：

AI 协助：

仍待核验：

主要错因：

任务状态变化：

能力状态变化：

是否影响本周 P0：

若新增范围，删除或降级了什么：

下一步第一动作：
```

## 6. Retest

```text
当天验收：

1 天短回忆：

3 天迁移任务：

7 天 A0 无辅助复现：
```

## 7. 快速模式调用示例

```text
/tutor A1，S 任务。请一次只问一个问题，先让我解释 TCP 为什么需要三次握手。
```

```text
/exam A0，L 任务。给我一组 60 分钟算法模拟题，中途不要提示，结束后统一评分。
```

```text
/review A2，M 任务。先对抗性审查我的异步任务方案，不要直接替我重写。
```

```text
/build A4，L 任务。先读取相关代码和验收标准，只实现一个 Tool Calling 纵向切片，运行测试并汇报 Diff。
```

```text
/interview A0，M 任务。模拟 AI 应用全栈面试，围绕项目动态追问，中途不教学。
```

```text
/archive。区分我独立完成和 AI 协助内容，更新状态，并留下 1/3/7 天无辅助复测。
```
