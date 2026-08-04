# 秋招准备知识库

> 版本：v2.2  
> 基准日期：2026-08-03  
> 当前日程起点：2026-08-04  
> 目标岗位：AI Agent 应用开发、AI 应用全栈、前端开发  
> 执行场景：工作日实习碎片时间为主，准备、投递、项目和复盘并行

> **AI 入口：**处理本目录任务前，必须先读取 [`AGENTS.md`](./AGENTS.md)。它定义用户基线、援助等级、协作模式、日程来源、完成标准和禁止行为。

## 1. 核心战略

这不是一套“学完再投”的课程表，而是一套持续产生求职证据的作战系统：

```text
岗位与投递反馈
        ↓
算法 / 计算机基础 / 工程能力
        ↓
可运行的 Agent 纵向切片
        ↓
简历、项目讲解与模拟面试
        ↓
真实笔试和面试反馈
        └────────────→ 调整下一轮 P0
```

岗位优先级：

1. **AI Agent 应用 / AI 应用全栈**：主投方向；
2. **全栈开发**：工程底座和重要投递方向；
3. **前端开发 / AI 前端**：已有优势和稳定投递方向。

不等待九月再开始投递。准备、投递、项目建设和面试复盘从现在起并行。

## 2. 当前风险

- 算法已刷约 200 题，但无标签识别、独立推导和间隔复现不稳定；
- 前端有项目经验，但长期依赖 AI Coding 后需要恢复独立手写和调试；
- 后端有真实业务实践，但计算机基础、可靠性和原理表达不系统；
- Agent 概念覆盖较多，但缺少可运行、可追踪、可评测的最小工程证据；
- 当前简历尚未完整纳入美团实习，且部分结论和指标需要事实审计；
- 原项目范围包含三语言、三服务、RAG、异步任务、Trace 和部署，四周内存在半成品风险；
- AI 可以提高工程速度，但若不限制援助等级，会掩盖算法、手写、系统判断和面试表达的真实缺口；
- 知识地图如果没有依赖、日期、记录和复测，只会形成“看起来全面”的待办堆积。

## 3. 当前投入比例

在 Week 0 诊断结束前使用以下临时权重：

| 流水线 | 权重 | 目标 |
| --- | ---: | --- |
| 算法与独立编码 | 35% | 无标签识别、Python 实现、ACM 输入输出和间隔复现 |
| Agent 项目与原理 | 25% | 单一后端栈完成 Tool + RAG + Trace + Eval 闭环 |
| 后端与计算机基础 | 20% | 网络、操作系统、数据库、请求链路和可靠性 |
| 简历、投递与面试 | 10% | 美团经历、双版本简历、持续投递和反馈闭环 |
| 前端维护 | 10% | JS/TS 手写、组件状态、性能和 AI 原生交互 |

Week 0 后按真实断点调整，不长期锁死固定比例。

## 4. 仓库导航

### AI 协作入口

- [`AGENTS.md`](./AGENTS.md)：供 AI 优先读取的强制协作、日程和权限规则；
- [`execution/human-ai-collaboration.md`](./execution/human-ai-collaboration.md)：面向人的详细协作手册；
- [`execution/task-template.md`](./execution/task-template.md)：通用 S/M/L 任务契约、援助记录、验收和复测模板。

### 日程与记录入口

- [`schedule/README.md`](./schedule/README.md)：日程执行方式、深度层级和完成定义；
- [`schedule/learning-sequence.md`](./schedule/learning-sequence.md)：算法、CS、后端、Agent、前端和求职知识依赖；
- [`schedule/calendar-2026-08-04-to-09-06.md`](./schedule/calendar-2026-08-04-to-09-06.md)：从 8 月 4 日到 9 月 6 日的逐日任务；
- [`schedule/progress-ledger.md`](./schedule/progress-ledger.md)：当前 P0、任务看板、能力深度、复测和证据总账；
- [`schedule/daily-log-template.md`](./schedule/daily-log-template.md)：每日可执行记录模板；
- [`schedule/weekly-review-template.md`](./schedule/weekly-review-template.md)：周指标、范围删除、反馈和下周 P0 模板。

### 战略与四条流水线

- [`00-strategy-and-positioning.md`](./00-strategy-and-positioning.md)：岗位边界、技术栈职责和停止清单；
- [`08-09-sprint-plan.md`](./08-09-sprint-plan.md)：8 月至 9 月初的并行冲刺周目标；
- [`application-pipeline.md`](./application-pipeline.md)：岗位收集、投递、状态和周指标；
- [`resume-strategy.md`](./resume-strategy.md)：美团经历、双版本简历和事实审计；
- [`interview-feedback-loop.md`](./interview-feedback-loop.md)：笔试、面试反馈如何反哺学习路线。

### 知识框架

- [`knowledge-framework/README.md`](./knowledge-framework/README.md)：知识树与 L1～L4 掌握等级；
- [`knowledge-framework/shared-foundation.md`](./knowledge-framework/shared-foundation.md)：算法、网络、操作系统、数据库、Linux 和软件工程；
- [`knowledge-framework/frontend.md`](./knowledge-framework/frontend.md)：JS/TS、浏览器、框架、工程化和 AI UI；
- [`knowledge-framework/backend.md`](./knowledge-framework/backend.md)：Java、Spring、数据、异步与可靠性；
- [`knowledge-framework/ai-agent.md`](./knowledge-framework/ai-agent.md)：模型基础、Agent Runtime、RAG、框架、评测和安全；
- [`knowledge-framework/project-and-interview.md`](./knowledge-framework/project-and-interview.md)：收缩后的项目 MVP 与三岗位叙事；
- [`knowledge-framework/learning-roadmap-v1.md`](./knowledge-framework/learning-roadmap-v1.md)：从诊断到反馈驱动补洞的阶段路线。

### 执行与复盘

- [`execution/README.md`](./execution/README.md)：工作日 S/M/L 任务系统；
- [`execution/week-0-baseline-2026-08-03.md`](./execution/week-0-baseline-2026-08-03.md)：第一周诊断和投递入口任务；
- [`04-algorithm-training-system.md`](./04-algorithm-training-system.md)：无标签、限时、间隔复现和模拟笔试体系；
- [`05-diagnosis-and-review-templates.md`](./05-diagnosis-and-review-templates.md)：单题、周复盘和面试表达模板。

历史概要 `01`～`03` 仅保留背景参考，执行以本页链接的 v2 文档、当前日期日程和总账为准。

## 5. 知识编排原则

所有主题统一按以下顺序推进：

```text
真实问题 / 具体样例
→ 最小实现或可观察现象
→ 关键机制和不变量
→ 失败模式与相邻概念
→ 抽象模型与方案取舍
→ 新场景迁移与面试表达
```

深度使用 D0～D4：

- D0：定位真实断点；
- D1：处理明确样例；
- D2：解释机制；
- D3：处理失败、比较方案和抽象；
- D4：迁移到陌生问题、系统设计和真实面试。

AI 不得跳过具体证据，直接用术语或高级讲解把主题标为掌握。

## 6. 学习状态

```text
TODO
→ LEARNING
→ CAN_EXPLAIN
→ CAN_IMPLEMENT
→ USED_IN_PROJECT
→ INTERVIEW_READY
```

阅读最多进入 `LEARNING`。AI 生成的答案、代码或文档不能直接升级能力状态；升级必须有无辅助口述、独立代码、测试、项目应用或模拟面试证据。

## 7. 人机协作原则

```text
人定义目标、首次推导、关键取舍和最终验收
+
AI 负责诊断、提示、反例、执行低学习价值工作和反馈整理
```

AI 协作采用 A0～A4 援助等级和 `/tutor`、`/exam`、`/interview`、`/review`、`/build`、`/archive` 六种模式。具体规则见 [`AGENTS.md`](./AGENTS.md)。

每次 AI 协作必须留下：

1. 人独立完成与 AI 协助内容的区分；
2. 仍待事实或测试核验的内容；
3. 下一步第一动作；
4. 至少一个未来的无 AI 验收或复测。

## 8. 项目范围护栏

首版项目只要求：

```text
前端输入
→ 单一后端服务
→ 文档检索
→ 一个只读工具
→ 模型回答与真实引用
→ Trace
→ 固定评测集
```

首版不默认建设 Java + Python 双服务，不默认引入 MQ、复杂 MCP、多 Agent、Rerank、Kubernetes 或拖拽工作流。

## 9. 当前立即执行

从当前日期日程开始，不再自行选择宽泛主题：

1. 打开 [`schedule/calendar-2026-08-04-to-09-06.md`](./schedule/calendar-2026-08-04-to-09-06.md)；
2. 检查 [`schedule/progress-ledger.md`](./schedule/progress-ledger.md) 的 `DUE`、`DOING` 和最多五个 P0；
3. 根据当天容量选择一个主任务；
4. 复制 [`schedule/daily-log-template.md`](./schedule/daily-log-template.md)；
5. 完成、验收、更新证据与 D+1/D+3/D+7 复测；
6. 周五使用 [`schedule/weekly-review-template.md`](./schedule/weekly-review-template.md) 调整下一周，不整体顺延未完成任务。

当前第一动作：执行 `W0-D1-ALG-01`，从旧题中随机抽取滑动窗口、二分、单调栈各一题，关闭题解和 AI 提示，进行无标签诊断。
