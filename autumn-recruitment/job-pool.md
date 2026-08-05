# 秋招岗位池

> 用途：记录真实岗位、反推学习模块，并持续维护投递状态。  
> 能力判断遵循 [`execution/zero-baseline-learning-policy.md`](./execution/zero-baseline-learning-policy.md)：未经当前周期独立验证的能力一律记为 `TODO / 未验证`。

## 记录规则

- 动态岗位信息以公司官方招聘页面为准；
- 岗位要求先用于反推学习模块，不因当前缺口暂停合理投递；
- 每条记录保留职位 ID、核验日期、状态和下一步；
- 超过七天未处理时重新核验岗位是否仍有效。

---

## JOB-2026-001 百度 2027AIDU-Agent 应用全栈工程师

```text
公司：百度
岗位：2027AIDU-Agent 应用全栈工程师
职位 ID：J99974
岗位类型：A（AI Agent 应用 / AI 应用全栈）
地点：北京
招聘项目：2027AIDU 校园招聘
官方发布日期：2026-07-21
最近核验：2026-08-05
来源：百度校园招聘官方页面
毕业资格：面向毕业时间在 2026-09-01 至 2027-08-31 的全球 2027 届毕业生；用户预计 2027 年 6 月毕业，资格匹配
截止时间：官方页面未标明，需在投递前重新核验
状态：READY_TO_APPLY / RESUME_NOT_READY
```

### 核心职责

1. 构建能够执行任务的 Autonomous Agent，而非仅完成一次对话；
2. 设计 Planning → Acting → Reflection 闭环；
3. 建设 Tool / API 调用、长短期 Memory、多轮推理与状态管理；
4. 推进 RAG 与 Agent 融合及真实业务落地；
5. 建设 Evaluation，优化成功率、稳定性、Token/调用成本、延迟和用户体验；
6. 岗位还涉及 Multi-Agent 与前沿方向探索。

### P0 要求

- 能够动手构建 AI Agent、自动化工具或智能助手项目；
- 深度使用大模型，并理解能力边界与局限；
- 理解 Agent Loop、Tool Calling、状态、Memory、RAG 和 Evaluation；
- 具备快速实验、迭代和工程落地能力；
- 使用过至少一种 Agent 框架，但框架名本身不构成能力证据。

### 加分项 / 扩展项

- Multi-Agent；
- Tool Learning、Self-Improvement、长期记忆、World Model、多模态 Agent；
- 在搜索、医疗、企业服务、数据分析或自动化办公等真实业务中落地。

### 反推学习模块

| 学习模块 | 前置依赖 | 当前状态 | 优先级 | 对应路线 |
| --- | --- | --- | --- | --- |
| Agent Loop 与显式状态 | 单次模型调用、Structured Output | LEARNING，尚无独立工程证据 | P0 | W0-D2-AG-01 → W0-D3-AG-01 |
| Tool Calling 与工具执行边界 | JSON Schema、参数校验、错误处理 | LEARNING / 未验证 | P0 | W1-D3-AG-01 → W1-D4-AG-01 |
| RAG 与真实 Citation | 文档切分、检索、引用映射 | TODO | P0 | 当前 Agent MVP 主链路 |
| Trace 与 Evaluation | 可观测状态、固定样例、成功判定 | TODO | P0 | 当前 Agent MVP 主链路 |
| Memory | 状态、上下文管理、存储边界 | TODO | P1 | 先完成短任务状态，再学习 Memory |
| Multi-Agent | 单 Agent Loop、Tool、Eval | TODO | Backlog | 首版范围明确暂缓 |
| 全栈产品落地 | 前端交互、后端 API、失败恢复 | 部分实践待事实审计 | P0 | 美团事实卡 + Agent MVP |

### 当前匹配判断

```text
方向匹配：高
校招资格：已确认匹配（预计 2027 年 6 月毕业）
当前证据匹配：未验证，不能按高匹配计算
综合判断：中匹配候选；值得尽快进入实际投递准备
我的匹配证据：未验证
主要缺口：没有已核验的 Agent MVP、Trace、Evaluation 和真实 Citation 证据
使用简历版本：AI 应用全栈版（尚未完成）
是否投递：建议完成最小事实审计与 AI 应用全栈简历骨架后尽快投递，不等待全部学习完成
```

### 下一步

1. 毕业资格已确认，不再阻塞投递；
2. 将该岗位保留为 A 类高优先级实际投递候选；
3. 不因岗位出现 Multi-Agent、长期 Memory 等扩展项而扩大当前项目首版；
4. 继续执行既定的单 Agent、一个只读 Tool、RAG、真实 Citation、Trace 和固定 Eval MVP；
5. AI 应用全栈版简历形成后，进行一次针对该岗位的事实匹配审查并重新核验岗位有效性。
