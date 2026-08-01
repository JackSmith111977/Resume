# 邱显煜

前端开发工程师 · 全栈开发工程师

- 邮箱：[3526547131@qq.com](mailto:3526547131@qq.com)
- 电话：13266338732
- 所在地：大连 · 佛山
- 个人网站：[https://keidesu.top](https://keidesu.top)
- GitHub：[JackSmith111977](https://github.com/JackSmith111977)

## 教育经历

### 大连理工大学

- 专业：软件工程
- 学历：本科 · 前30%
- 地点：大连
- 时间：2023-09 – 2027-08

## 技能

| 类别 | 技术 |
| --- | --- |
| 编程语言 | JavaScript、TypeScript、HTML、CSS |
| 前端框架 | React 18/19、Next.js 15/16、Taro 3/4 |
| 状态管理 | Zustand |
| 测试工具 | Vitest、Playwright MCP、Next.js DevTools MCP |
| 后端基础 | Node.js、Server Actions、BFF、API Route |
| 数据库 | Supabase（PostgreSQL）、MongoDB |
| DevOps | Git、GitHub Actions |
| Vibe Coding | Trae、Claude Code、文档优先开发、Skill 开发、上下文工程 |

## 项目经历

### 易盾-酒店预订与多端管理平台

**时间：**2026.02 – 至今

**职责：**架构设计师、核心开发者  
**项目协作：**三人团队 · 分模块合作开发 · 携程前端训练营项目

**项目背景：**为中小型酒店提供从 B 端管理到 C 端预订的一体化解决方案，覆盖 PC Web 管理端、微信小程序用户预订端，支持酒店入驻审核、房型管理、在线预订全流程。

**技术栈：**Next.js 16、React 19、TypeScript、Taro 4.x、Supabase、Zustand、Tailwind CSS v4

**核心贡献：**

- **多端架构设计：**整个项目采用 Serverless 架构，PC 端采用 Next.js 全栈框架，移动端采用 Taro 跨端开发，Supabase 作为数据库，是双端的唯一真实来源。利用 Supabase 这类 BaaS 服务，使团队更注重前端业务实现，降低后端维护压力，提高后端开发效率。
- **中间层设计：**PC 端采用 Server Actions 作为中间层与 Supabase 交互。由于 Server Actions 运行在服务端，保证了环境变量安全性；移动端采用微信云函数作为中间层，云函数运行在微信小程序的隔离环境中，环境变量不暴露在前端，从根本上防范了 XSS 注入攻击。
- **Next.js 框架优化：**利用 Next.js 提供的多种渲染服务，精确设计不同的组件：静态组件采用 SSG 渲染，服务端组件根据业务使用 SSR 或 ISR 渲染，只有使用 React Hooks 和浏览器 API 的组件被设计为客户端渲染，将首屏加载时间控制在 1.2s 内。
- **Taro 跨端开发：**通过配置式分包，将主包的体积控制在 1.6MB 以内。
- **全局状态管理：**使用 Zustand 替代 React Context API，采用外置 store 进行统一的全局状态管理，减少大量模板代码，降低维护成本。
- **长列表优化：**利用小程序原生的交叉观察器和二维数组将数据分片，实现自定义的虚拟列表，配合骨架屏占位，实现稳定高性能的定高虚拟列表。
- **RPC 函数开发：**利用 RPC 函数实现后端数据库的复杂查询和处理逻辑，将数据处理下放到后端环境完成，提升前端的渲染性能和数据获取效率。

**项目地址：**[https://github.com/JackSmith111977/Yisu-Hotel-Booking-Platform-PC](https://github.com/JackSmith111977/Yisu-Hotel-Booking-Platform-PC)

### StyleSnap-网页设计风格参考平台

**时间：**2026.03 – 至今

**职责：**独立开发者 · 文档生成构建 · 顶层架构设计 · Skill 开发

**项目背景：**帮助前端开发者快速选择、理解和应用网页开发视觉风格的一站式平台。

**开发模式：**文档优先 · Claude Code · AI 多智能体协同

**核心贡献：**

- **文档优先模式实践：**在编码前按照软件工程，通过无限询问机制创建完整的文档体系，包括 PRD（产品需求）、APP_FLOW（应用流程）、TECH_STACK（技术栈）、FRONTEND_GUIDELINES（前端规范）等 6 大核心文档，确保开发方向清晰，降低 AI 幻觉，减少返工率。
- **AI 多智能体协同开发：**配置 6 个专业 Sub-agents（架构师、前端、后端、数据库、测试、文档），通过 Git 分支隔离实现并行开发，开发效率提升。
- **上下文隔离机制：**每个 Agent 独立上下文窗口，避免 Token 爆炸和上下文污染，单次会话 Token 消耗降低。
- **技术选型与架构：**采用 Next.js 16 App Router + Supabase BaaS 方案，利用 Server Actions 替代传统 API 路由，减少代码量。
- **知识沉淀：**创建 15+ 技术核心知识文档（Next.js、Supabase、Zustand 等），每个技术点包含概念定义、工作原理、源码解析、最佳实践。

**项目地址：**[https://github.com/JackSmith111977/StyleSnap](https://github.com/JackSmith111977/StyleSnap)

## 其他经历

- **腾讯广告-大咖精英班**（2025）  
  完成课程大作业，顺利结项。
- **字节跳动工程训练营-前端**（2025）  
  完成课程大作业，并顺利结项。
- **携程第五期前端训练营**（2026）  
  完成课程大作业，通过大作业答辩，顺利结项。

## 奖项

- 动感地带 AI+ 高校创新设计技术赛道东北赛区三等奖（2025）
- APMCM 亚太地区大学生数学建模竞赛三等奖（2023）
