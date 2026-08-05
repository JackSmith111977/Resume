# 2026-08-05 时间护栏规则修订

## 1. 触发

用户反馈：按计划时间立即中断会影响集中，更合理的方式应是时间到点提醒，并完成当前章节或当前认知闭环后结束。

AI 与用户进一步澄清：不能把“完成整个章节”作为无限加时依据。规则应改为：

```text
计划预算到点
→ 软停止提醒一次
→ 冻结范围，不再开启新概念或新问题
→ 在有限缓冲内完成当前预定义闭合单元
→ 到达绝对停止后必须归档
```

## 2. 根因

旧规则只有“硬停止点”，混合了两个不同目的：

- 防止范围无限扩张；
- 决定何时中断当前交互。

这导致两种相反偏差：

1. `CURR-FND-01-S1` 中没有及时关闭范围，15 分钟课程扩展到 37 分钟；
2. `CURR-FND-01-S2` 中又机械按时间尝试中断当前复述，并发生一次时间误判。

## 3. 新规则

### 三级边界

```text
计划工作预算 / 软停止
→ 闭环缓冲
→ 绝对停止
```

### 闭合单元

闭合单元必须在任务开始前定义，并小于一整个章节、功能、题组或路线阶段。

教学任务的典型闭合单元：

```text
当前问题的用户回答
→ 必要纠正
→ 一次自己的话复述或局部验证
→ 知识卡与未理解点
```

### 默认缓冲

```text
S：最多 5 分钟
M：最多 5～10 分钟
L：最多 10 分钟
```

缓冲计入任务总时长和当天单领域预算，不是额外无限加时。

### 软停止后禁止

- 新的苏格拉底问题；
- 新概念、新机制和新反例链；
- 下一题、下一章、下一岗位或下一功能；
- 多次时间提醒打断用户推理。

### 绝对停止

闭环缓冲耗尽、单领域上限到达或归档时间受威胁时，保存可审查状态并停止，即使闭环仍不完美。

## 4. 修改文件

- `/AGENTS.md`
- `/autumn-recruitment/AGENTS.md`
- `/autumn-recruitment/execution/time-budget-and-task-guardrails.md`
- `/autumn-recruitment/execution/systematic-zero-baseline-teaching-policy.md`
- `/autumn-recruitment/schedule/progress-ledger.md`

## 5. 后续 Task Contract 必填

```text
计划工作预算 / 软停止：
预定义闭合单元：
闭环缓冲：
绝对停止：
软停止后明确不做：
```

## 6. 规则验收

后续任务结束记录必须包含：

```text
Planned working budget / soft stop:
Declared closure unit:
Closure buffer:
Soft stop reached:
Closure work after soft stop:
Absolute stop reached:
```

## 7. 当前结论

> 时间规则限制的是范围扩张，而不是在预算刚到时机械打断当前思考；但完成当前闭环也不能成为继续整章或相邻主题的理由。
