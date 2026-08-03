# 秋招准备知识库

> 创建日期：2026-08-03  
> 目标岗位：AI Agent 应用开发、全栈开发、前端开发  
> 学习场景：以工作日实习期间的碎片时间为主，不依赖周末集中学习

## 1. 求职定位

当前采用一条共享主干，而不是分别学习三套割裂的技术体系：

```text
算法与计算机基础
→ 软件工程与独立编码
→ 前端交互 + 后端业务
→ AI Agent 工程化
→ 项目、简历与面试证据
```

岗位优先级：

1. **AI Agent 应用开发**：主投方向；
2. **全栈开发**：核心工程底座与重要投递方向；
3. **前端开发**：已有相对优势，作为稳定投递方向。

详细决策见 [`00-strategy-and-positioning.md`](./00-strategy-and-positioning.md)。

## 2. 当前能力基线

- 前端：相对熟悉，有 React / Next.js / Vue / TypeScript 项目实践；
- 后端：有全栈和真实业务经验，但系统性、可靠性与原理表达需要补足；
- Agent：了解应用概念，需要补运行时、RAG、评测、Trace 和安全；
- 算法与手写代码：当前最大风险；
- 算法主语言：**Python**；
- 已刷约 200 道题，主要按照灵茶山艾府题单专题学习；
- 主要问题：间隔重做中等题时依赖原题解记忆，尚未形成稳定的独立推导能力。

## 3. 当前时间分配

| 方向 | 初始权重 | 阶段目标 |
| --- | ---: | --- |
| 算法与独立编码 | 50% | 无标签识别、独立推导和 Python 实现 |
| 后端核心链路 | 25% | API、数据、异步、幂等、重试和可观测性 |
| Agent 底层机制 | 20% | 手写可恢复、可追踪、可评测的最小 Agent |
| 前端维护 | 5% | 保持优势并补 AI 原生交互能力 |

算法达到基础门槛后，把更多时间转移到 Agent 项目、后端系统设计和面试表达。

## 4. 仓库导航

### 战略与阶段路线

- [`00-strategy-and-positioning.md`](./00-strategy-and-positioning.md)：岗位选择、技术栈职责和投入边界；
- [`08-09-sprint-plan.md`](./08-09-sprint-plan.md)：8 月到 9 月初的工作日碎片化冲刺计划；
- [`knowledge-framework/learning-roadmap-v1.md`](./knowledge-framework/learning-roadmap-v1.md)：从诊断到投递的阶段路线。

### 详细知识框架

- [`knowledge-framework/README.md`](./knowledge-framework/README.md)：知识树和 L1～L4 掌握等级；
- [`knowledge-framework/shared-foundation.md`](./knowledge-framework/shared-foundation.md)：算法、网络、操作系统、数据库与软件工程；
- [`knowledge-framework/frontend.md`](./knowledge-framework/frontend.md)：前端核心、工程化与 AI 原生交互；
- [`knowledge-framework/backend.md`](./knowledge-framework/backend.md)：Java、Spring、数据、异步任务和可靠性；
- [`knowledge-framework/ai-agent.md`](./knowledge-framework/ai-agent.md)：Agent Loop、Tool、RAG、MCP、Evaluation 和安全；
- [`knowledge-framework/project-and-interview.md`](./knowledge-framework/project-and-interview.md)：项目、简历和三岗位面试闭环。

### 执行与复盘

- [`execution/README.md`](./execution/README.md)：工作日 S/M/L 任务系统、AI 使用边界和周指标；
- [`execution/week-0-baseline-2026-08-03.md`](./execution/week-0-baseline-2026-08-03.md)：第一周能力诊断看板；
- [`04-algorithm-training-system.md`](./04-algorithm-training-system.md)：针对模式识别和题解记忆的算法训练体系；
- [`05-diagnosis-and-review-templates.md`](./05-diagnosis-and-review-templates.md)：单题、混合诊断与周复盘模板。

### 历史概要

以下文档保留作为早期总结，后续以 `knowledge-framework/` 和 `execution/` 为准：

- [`01-role-knowledge-map.md`](./01-role-knowledge-map.md)；
- [`02-current-profile-and-gaps.md`](./02-current-profile-and-gaps.md)；
- [`03-minimum-learning-roadmap.md`](./03-minimum-learning-roadmap.md)。

## 5. 学习状态标准

```text
TODO
→ LEARNING
→ CAN_EXPLAIN
→ CAN_IMPLEMENT
→ USED_IN_PROJECT
→ INTERVIEW_READY
```

阅读和观看课程最多进入 `LEARNING`。只有通过口述、独立编码、项目应用或模拟面试验收，才能继续升级。

## 6. 执行原则

- 所有任务拆成 10～45 分钟的独立检查点；
- 每次结束留下可以直接执行的下一步；
- 算法首轮分析和编码不让 AI 直接生成答案；
- 项目可以使用 AI Coding，但必须有人工作方案、测试、Diff 审查和失败验证；
- 不按学习时长和刷题数评估，按可解释、可实现、可工程化和可面试评估；
- 周末不承担强制任务，只作为休息或可选缓冲；
- 模型、框架、协议和岗位要求等动态信息在投递前重新核验官方来源。

## 7. 当前下一步

执行 [`execution/week-0-baseline-2026-08-03.md`](./execution/week-0-baseline-2026-08-03.md)，得到：

1. 算法六专题真实断点；
2. 后端异步任务链路缺口；
3. Agent Loop 概念与工程缺口；
4. 下一周最多五个 P0 任务。
