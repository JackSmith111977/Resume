# LeetCode 秋招算法题单 v2

> 基线：历史上做过约 200 题，但已停练约两个月；本轮统一按“未掌握”从头重建。  
> 主语言：Python。  
> 目标：先理解具体操作和状态变化，再独立实现，最后进入无标签识别和限时模拟。

## 1. 训练规则

### 新主题不得直接考试

每个新模式按以下顺序推进：

```text
概念预测
→ 锚点题讲解与手算
→ 引导实现
→ 同类题独立实现
→ D+1 复述
→ D+3 核心代码
→ D+7 无标签完整复现
→ 混合题池
```

- 锚点题：`/tutor`，默认 A1，卡住后最多 A2；
- 引导题：`/tutor` A1/A2，用户先写暴力、状态和边界；
- 独立题：先 A0，10 分钟后仍无方向才升级 A1；
- 前两周不以无标签识别率作为主要指标；
- AI 给出的完整代码不计为完成；
- 历史上见过题目不自动跳过，当前无辅助证据才算掌握。

### 完成标记

| 标记 | 含义 |
| --- | --- |
| `ANCHOR` | 用于学习模式和观察状态变化 |
| `GUIDED` | 在 A1/A2 下完成推导和实现 |
| `INDEPENDENT` | 首轮无关键提示完成 |
| `TRANSFER` | 条件变化或混合场景迁移 |
| `STRETCH` | 困难扩展，不阻塞主线 |

---

## 2. Phase 0：Python、数组与最小思维闭环

> 先恢复 `dict`、`set`、列表、循环、边界、复杂度和手动测试。不要一开始同时学习多个高级模式。

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| P0-01 | 1 | 两数之和 | 简单 | ANCHOR | 暴力重复计算；哈希表保存什么 | https://leetcode.cn/problems/two-sum/ |
| P0-02 | 217 | 存在重复元素 | 简单 | GUIDED | `set`、提前返回、空间换时间 | https://leetcode.cn/problems/contains-duplicate/ |
| P0-03 | 242 | 有效的字母异位词 | 简单 | INDEPENDENT | 计数表、频次不变量 | https://leetcode.cn/problems/valid-anagram/ |
| P0-04 | 704 | 二分查找 | 简单 | ANCHOR | 区间定义与循环不变量 | https://leetcode.cn/problems/binary-search/ |
| P0-05 | 20 | 有效的括号 | 简单 | ANCHOR | 栈保存尚未匹配的状态 | https://leetcode.cn/problems/valid-parentheses/ |

### Phase 0 通过条件

- 能从空文件写出 Python 函数和至少两个测试；
- 能解释时间、空间复杂度；
- 能说清容器中保存的信息，而不是只背代码；
- `P0-01`、`P0-03`、`P0-04` 至少各完成一次 D+7。

---

## 3. Phase 1：哈希、双指针与滑动窗口

### 3.1 哈希与前缀状态

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| HT-01 | 49 | 字母异位词分组 | 中等 | GUIDED | 设计可哈希的分组键 | https://leetcode.cn/problems/group-anagrams/ |
| HT-02 | 128 | 最长连续序列 | 中等 | INDEPENDENT | 只从序列起点扩展 | https://leetcode.cn/problems/longest-consecutive-sequence/ |
| HT-03 | 560 | 和为 K 的子数组 | 中等 | TRANSFER | 前缀和与历史状态计数 | https://leetcode.cn/problems/subarray-sum-equals-k/ |

### 3.2 双指针

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| TP-01 | 125 | 验证回文串 | 简单 | ANCHOR | 两端指针和跳过无效字符 | https://leetcode.cn/problems/valid-palindrome/ |
| TP-02 | 27 | 移除元素 | 简单 | GUIDED | 读写指针与原地覆盖 | https://leetcode.cn/problems/remove-element/ |
| TP-03 | 283 | 移动零 | 简单 | INDEPENDENT | 稳定移动与写指针 | https://leetcode.cn/problems/move-zeroes/ |
| TP-04 | 11 | 盛最多水的容器 | 中等 | TRANSFER | 为什么移动短板才可能变优 | https://leetcode.cn/problems/container-with-most-water/ |

### 3.3 滑动窗口

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| SW-01 | 209 | 长度最小的子数组 | 中等 | ANCHOR | 扩张、收缩和窗口合法条件 | https://leetcode.cn/problems/minimum-size-subarray-sum/ |
| SW-02 | 3 | 无重复字符的最长子串 | 中等 | GUIDED | 窗口内频次与左端移动 | https://leetcode.cn/problems/longest-substring-without-repeating-characters/ |
| SW-03 | 438 | 找到字符串中所有字母异位词 | 中等 | INDEPENDENT | 固定窗口与计数差异 | https://leetcode.cn/problems/find-all-anagrams-in-a-string/ |
| SW-04 | 567 | 字符串的排列 | 中等 | TRANSFER | 与 438 比较输出条件 | https://leetcode.cn/problems/permutation-in-string/ |
| SW-X1 | 76 | 最小覆盖子串 | 困难 | STRETCH | 多重约束和最小合法窗口 | https://leetcode.cn/problems/minimum-window-substring/ |

---

## 4. Phase 2：链表、栈与二分

### 4.1 链表

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| LL-01 | 206 | 反转链表 | 简单 | ANCHOR | 指针重连前保存后继 | https://leetcode.cn/problems/reverse-linked-list/ |
| LL-02 | 21 | 合并两个有序链表 | 简单 | GUIDED | 虚拟头节点和推进条件 | https://leetcode.cn/problems/merge-two-sorted-lists/ |
| LL-03 | 141 | 环形链表 | 简单 | INDEPENDENT | 快慢指针为何必然相遇 | https://leetcode.cn/problems/linked-list-cycle/ |
| LL-04 | 160 | 相交链表 | 简单 | TRANSFER | 两指针路径长度对齐 | https://leetcode.cn/problems/intersection-of-two-linked-lists/ |
| LL-05 | 19 | 删除链表的倒数第 N 个结点 | 中等 | GUIDED | 固定间距与虚拟头节点 | https://leetcode.cn/problems/remove-nth-node-from-end-of-list/ |
| LL-06 | 2 | 两数相加 | 中等 | TRANSFER | 进位状态和不同长度 | https://leetcode.cn/problems/add-two-numbers/ |

### 4.2 栈与单调栈

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| ST-01 | 155 | 最小栈 | 中等 | GUIDED | 主栈与辅助状态同步 | https://leetcode.cn/problems/min-stack/ |
| ST-02 | 739 | 每日温度 | 中等 | ANCHOR | 栈中保存“尚未找到答案”的下标 | https://leetcode.cn/problems/daily-temperatures/ |
| ST-03 | 496 | 下一个更大元素 I | 简单 | INDEPENDENT | 单调栈结果映射 | https://leetcode.cn/problems/next-greater-element-i/ |
| ST-X1 | 84 | 柱状图中最大的矩形 | 困难 | STRETCH | 左右边界与弹栈时机 | https://leetcode.cn/problems/largest-rectangle-in-histogram/ |

### 4.3 二分

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| BS-01 | 35 | 搜索插入位置 | 简单 | GUIDED | 二分边界与插入位置 | https://leetcode.cn/problems/search-insert-position/ |
| BS-02 | 34 | 在排序数组中查找元素的第一个和最后一个位置 | 中等 | INDEPENDENT | 左边界与右边界统一写法 | https://leetcode.cn/problems/find-first-and-last-position-of-element-in-sorted-array/ |
| BS-03 | 153 | 寻找旋转排序数组中的最小值 | 中等 | GUIDED | 保留答案所在有序区间 | https://leetcode.cn/problems/find-minimum-in-rotated-sorted-array/ |
| BS-04 | 33 | 搜索旋转排序数组 | 中等 | TRANSFER | 判断哪一半有序并排除 | https://leetcode.cn/problems/search-in-rotated-sorted-array/ |

---

## 5. Phase 3：树、图、回溯与堆

### 5.1 二叉树

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| TREE-01 | 104 | 二叉树的最大深度 | 简单 | ANCHOR | 递归函数语义 | https://leetcode.cn/problems/maximum-depth-of-binary-tree/ |
| TREE-02 | 226 | 翻转二叉树 | 简单 | GUIDED | 子问题和返回值 | https://leetcode.cn/problems/invert-binary-tree/ |
| TREE-03 | 102 | 二叉树的层序遍历 | 中等 | ANCHOR | 队列与逐层边界 | https://leetcode.cn/problems/binary-tree-level-order-traversal/ |
| TREE-04 | 94 | 二叉树的中序遍历 | 简单 | INDEPENDENT | 递归与显式栈 | https://leetcode.cn/problems/binary-tree-inorder-traversal/ |
| TREE-05 | 98 | 验证二叉搜索树 | 中等 | GUIDED | 上下界约束而非只比较父子 | https://leetcode.cn/problems/validate-binary-search-tree/ |
| TREE-06 | 543 | 二叉树的直径 | 简单 | TRANSFER | 返回值与全局答案不同 | https://leetcode.cn/problems/diameter-of-binary-tree/ |

### 5.2 图与网格搜索

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| GRAPH-01 | 200 | 岛屿数量 | 中等 | ANCHOR | 连通分量和访问状态 | https://leetcode.cn/problems/number-of-islands/ |
| GRAPH-02 | 994 | 腐烂的橘子 | 中等 | GUIDED | 多源 BFS 与层数 | https://leetcode.cn/problems/rotting-oranges/ |
| GRAPH-03 | 133 | 克隆图 | 中等 | TRANSFER | 图遍历与旧节点到新节点映射 | https://leetcode.cn/problems/clone-graph/ |

### 5.3 回溯

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| BT-01 | 46 | 全排列 | 中等 | ANCHOR | 选择、撤销和路径状态 | https://leetcode.cn/problems/permutations/ |
| BT-02 | 78 | 子集 | 中等 | GUIDED | 每个位置选或不选 | https://leetcode.cn/problems/subsets/ |
| BT-03 | 39 | 组合总和 | 中等 | TRANSFER | 可重复选择和剪枝 | https://leetcode.cn/problems/combination-sum/ |

### 5.4 堆

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| HEAP-01 | 215 | 数组中的第 K 个最大元素 | 中等 | ANCHOR | 小顶堆维护 K 个候选 | https://leetcode.cn/problems/kth-largest-element-in-an-array/ |
| HEAP-02 | 347 | 前 K 个高频元素 | 中等 | GUIDED | 计数与 Top K 组合 | https://leetcode.cn/problems/top-k-frequent-elements/ |
| HEAP-X1 | 23 | 合并 K 个升序链表 | 困难 | STRETCH | 多路归并和堆元素设计 | https://leetcode.cn/problems/merge-k-sorted-lists/ |

---

## 6. Phase 4：动态规划、贪心与区间

### 6.1 动态规划

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| DP-01 | 70 | 爬楼梯 | 简单 | ANCHOR | 状态、转移、初值 | https://leetcode.cn/problems/climbing-stairs/ |
| DP-02 | 746 | 使用最小花费爬楼梯 | 简单 | GUIDED | 状态语义变化 | https://leetcode.cn/problems/min-cost-climbing-stairs/ |
| DP-03 | 198 | 打家劫舍 | 中等 | INDEPENDENT | 选或不选的最优子结构 | https://leetcode.cn/problems/house-robber/ |
| DP-04 | 322 | 零钱兑换 | 中等 | GUIDED | 完全背包、不可达状态 | https://leetcode.cn/problems/coin-change/ |
| DP-05 | 300 | 最长递增子序列 | 中等 | TRANSFER | 以当前位置结尾的状态 | https://leetcode.cn/problems/longest-increasing-subsequence/ |
| DP-06 | 1143 | 最长公共子序列 | 中等 | TRANSFER | 二维状态和字符匹配 | https://leetcode.cn/problems/longest-common-subsequence/ |
| DP-X1 | 416 | 分割等和子集 | 中等 | STRETCH | 0/1 背包与遍历顺序 | https://leetcode.cn/problems/partition-equal-subset-sum/ |

### 6.2 贪心与区间

| ID | 题号 | 题目 | 难度 | 角色 | 核心目标 | 链接 |
| --- | ---: | --- | --- | --- | --- | --- |
| GR-01 | 121 | 买卖股票的最佳时机 | 简单 | ANCHOR | 维护历史最小值 | https://leetcode.cn/problems/best-time-to-buy-and-sell-stock/ |
| GR-02 | 55 | 跳跃游戏 | 中等 | GUIDED | 最远可达边界 | https://leetcode.cn/problems/jump-game/ |
| INT-01 | 56 | 合并区间 | 中等 | GUIDED | 排序后的局部合并不变量 | https://leetcode.cn/problems/merge-intervals/ |
| GR-X1 | 45 | 跳跃游戏 II | 中等 | STRETCH | 分层贪心与当前覆盖范围 | https://leetcode.cn/problems/jump-game-ii/ |

---

## 7. 当前五周使用顺序

### Week 0：恢复最小闭环

1. `P0-01` 两数之和：讲解、手算、实现；
2. `P0-02` 存在重复元素；
3. `P0-03` 有效的字母异位词；
4. `TP-01` 验证回文串；
5. `P0-04` 二分查找；
6. `P0-05` 有效的括号。

### Week 1：哈希、双指针、窗口、栈

- `HT-01`、`TP-02`、`TP-03`、`SW-01`、`SW-02`、`ST-01`、`ST-02`；
- 周末可选完成 45 分钟小型复测，不做 90 分钟混合模拟。

### Week 2：链表与二分

- `LL-01`～`LL-05`；
- `BS-01`～`BS-03`；
- 将 Week 0 已学题混入 D+7 无标签复现。

### Week 3：树、图、回溯、堆

- `TREE-01`～`TREE-05`；
- `GRAPH-01`、`GRAPH-02`；
- `BT-01`、`BT-02`；
- `HEAP-01`。

### Week 4：DP、迁移与第一轮真实模拟

- `DP-01`～`DP-04`；
- `GR-01`、`INT-01`；
- 从已经完成 D+7 的题中组成第一次 60～90 分钟混合模拟；
- 未完成的高级题不形成欠债，按面试反馈决定是否继续。

---

## 8. 复测规则

```text
D+1：不看代码，复述问题、暴力、状态和不变量
D+3：写核心循环、递归语义或状态转移
D+7：从空文件完整实现并自测
D+14：隐藏专题，混入同阶段题池
```

- 锚点题讲解后也必须复测；
- D+7 失败则回到 `GUIDED`，不是反复背答案；
- 连续两次无关键提示完成后，才进入混合题池；
- 困难题和 `STRETCH` 不影响阶段通过。

## 9. 题目替换规则

只在以下情况替换：

- 题目因平台状态不可用；
- 与当前题高度重复且不能提供新的状态变化；
- 真实笔试或面试反馈要求加入更高优先级题型。

不能因为“以前做过”“看起来太简单”或“记得一点答案”而跳过。当前能力只由本轮无辅助证据决定。