# 王泽栋 · AI 产品经理

**AI 应用 / Agent / AI 电商 · 从 0 到 1 落地,评测驱动,结果导向**

浙江农林大学 · 智慧农业本科生(2023.09–2027.06) · 杭州 · 校招求职中

> 我关注的问题:**如何把大模型能力变成可用、可评测、可持续迭代,并且真正服务业务结果的产品。**

<p align="center">
  <img src="https://img.shields.io/badge/评测集-20%E4%BE%8B%20Benchmark-6f42c1" alt="评测集">
  <img src="https://img.shields.io/badge/Agent%20通过率-V1.0%2072%25%E2%86%92V1.1%2092%25-2ea44f" alt="Agent通过率">
  <img src="https://img.shields.io/badge/平台可用性-99.9%25-0052cc" alt="平台可用性">
  <img src="https://img.shields.io/badge/作品集-12%20%E4%B8%AA%E5%8F%AF%E5%85%AC%E5%BC%80%E4%BB%93%E5%BA%93-24292f" alt="作品集">
</p>

> 说明:主页中的业务数据已做去标识、区间化或相对化处理;面试时可以在合适的保密边界内展开具体项目背景与口径。

---

## 🎯 一句话

做过 AIGC 内容生产平台的商业化落地、电商导购 Agent 的效果治理、多个从调研到评测的 AI 产品原型;所有项目都遵循同一套方法——**先理解业务,再设计 AI;先定义评测,再追求效果;先做可用闭环,再扩展复杂能力。**

---

## 🏆 重点项目(结果先行)

### 1. [Mago AIGC Platform](https://github.com/cangyuyi/Mago-AIGC-Platform) — 聚合型 AIGC 内容生产平台 · 产品负责人

> 多模型聚合 + 场景化封装 + 多 Agent 协作 · 从 0 到 1 · **生产环境连续盈利**

**结果**:6 个月验证 PMF、连续盈利;峰值日生成 20 万+ 张,日均 8–12 万张;单位算力成本比官方直连低 40%;99.9% 企业级可用性;付费企业月复购 75%+;LTV/CAC > 30。

**我做了什么**:

- 深度访谈创作者与企业客户,提炼 API 不稳定、并发卡顿、场景脱节等关键痛点
- 规划绘图、视频、画布、电商、素材库五大模块,负责电商场景与前端产品落地
- 设计"热点情报 → 创意发散 → 脚本创作 → 角色/风格 → 提示词生成 → 一键生成"产品闭环
- 设计 8 个 Agent 协作的脚本工作流,沉淀 Prompt 模板、知识库与人工确认机制
- 用模型选型、Prompt 迭代、重试/反馈/阈值/归因/修复,平衡效果、稳定性与成本

**面试可展开**:用户研究、MVP 取舍、模型路由、工作流编排、容错设计、可观测性、定价与毛利。

<p align="center">
  <img src="https://raw.githubusercontent.com/cangyuyi/Mago-AIGC-Platform/main/screenshots/03-mago-canvas-workflow.png" alt="Mago 工作流画布" width="48%" />
  <img src="https://raw.githubusercontent.com/cangyuyi/Mago-AIGC-Platform/main/screenshots/04-mago-ecommerce-workstation.png" alt="Mago 电商工作台" width="48%" />
</p>

📌 [产品 README](https://github.com/cangyuyi/Mago-AIGC-Platform#readme) · [用户研究](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/01-user-research-summary.md) · [Prompt 迭代 SOP](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/02-prompt-iteration-sop.md) · [容错与降级](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/03-error-handling-mechanism.md) · [定价与毛利](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/04-pricing-and-margin.md)

---

### 2. 头部电商平台 AI 导购 Agent · 知识库 / Prompt / 评测闭环

> 面向真实电商咨询场景的 AI 产品迭代案例 · **评测驱动,效果可证明**

**结果**:脱敏后商品匹配准确率提升约 **15 个百分点**,参数类 Bad Case **下降约六成**,满意度明显提升;咨询转化与 AI 自主解决率提升,人工转接率明显下降。

**我做了什么**:

- 重构商品知识库:四类知识分库、标签体系、切片策略、SLA 与六步更新 SOP
- 设计 6 套导购 Prompt 模板,建立版本管理与离线评测机制
- 搭建转化率、人工转接率、响应时长、满意度等全维度指标看板
- 用"表现层 → 策略层 → 数据层 → 模型层"四层方法定位 Bad Case,按优先级推动修复

**面试可展开**:为什么先修知识库而不是先调模型、如何建立评测集、如何证明指标提升、如何处理大促风险。

---

### 3. [电视选购 Copilot](https://github.com/cangyuyi/tv-buying-copilot) — 纯 Python 自研 Multi-Agent 导购系统 · 独立原型

> 从零自研的电商导购 Agent 全流程独立重做版 · 含 PRD、评测、MCP

**结果**:25 条评测集驱动一轮迭代,通过率 **V1.0 72% → V1.1 92%**,幻觉次数 4 → 0,异常输入零崩溃。

- 四层架构:Master Router + 5 Skill Worker + Replanner + Compliance,高风险售后强制转人工
- 内置 MCP 工具服务(商品检索 / 促销计算 / 履约查询 / 售后政策),零第三方依赖,clone 即跑

📌 [AI_PRD](https://github.com/cangyuyi/tv-buying-copilot/blob/main/AI_PRD.md) · [V1.0 评测报告](https://github.com/cangyuyi/tv-buying-copilot/blob/main/evaluation/eval-results-v1.md) · [V1.1 评测报告](https://github.com/cangyuyi/tv-buying-copilot/blob/main/evaluation/eval-results-v1.1.md)

---

### 4. [AI PM Resume Writing](https://github.com/cangyuyi/ai-pm-sop) — AI 产品经理简历写作 Skill

> 把"简历诊断与改写"产品化为可复用的 AI 工作流

- JD 解析、证据映射、STAR/XYZ 改写、多版本定位,拆解复杂需求
- 七维诊断框架:关键词覆盖 / 经历相关性 / 量化充分性 / 证据一致性 / 定位一致性 / 时间线真实性 / 排版扫读友好度
- 针对 AI 应用/Agent、AI 增长、AI 策略/商业化三类岗位设计差异化输出
- 设置"不编造数据、不改原事实、不动原版式"的安全底线,处理生成式产品的可信度问题

📌 [方法论与使用说明](https://github.com/cangyuyi/ai-pm-sop#readme)

---

### 5. [BossHunter](https://github.com/cangyuyi/BossHunter) — AI 求职自动化产品

> 面向求职者的岗位发现、筛选、评分与投递辅助工作流 · 长期实践项目

重点关注:岗位信息采集、用户偏好配置、AI 评分、人工确认、投递队列、失败恢复与操作安全。**所有投递必须人工确认,不绕过平台安全机制。**

**面试可展开**:高风险自动化的人工确认、任务可恢复性、策略与体验的平衡、隐私与安全边界。

---

## 🧪 更多作品(每个都有仓库、评测或 Demo)

| 项目 | 一句话 | 亮点 |
| --- | --- | --- |
| [商策 Agent](https://github.com/cangyuyi/shance-commerce-agent-portfolio) | 电商营销内容 Agent 作品集 | 20 例 Benchmark,同一套评测对比单次 Prompt / 结构化 Prompt / Agent 工作流 |
| [瑞幸用户运营 Agent](https://github.com/cangyuyi/lucky-growth-agent) | 2026 AI 先锋大赛 · 瑞幸命题 | 意图识别 + 生命周期策略 + 置信度分级,DSL 可自部署 |
| [报销票据风险审核](https://github.com/cangyuyi/invoice-risk-review-agent) | 企业报销风险审核原型 | 二维码/OCR/视觉三路提取 + 确定性规则 + 人工兜底,含交互 Demo |
| [MSDS 职业危害识别](https://github.com/cangyuyi/msds-hazard-agent) | 唯享科技 AI 测试实习复盘重做 | [在线 Demo](https://msds-hazard-agent.streamlit.app/) · OCR + RAG + 人工复核,V1→V2 三轮迭代 |
| [火花工坊 HUB](https://github.com/cangyuyi/huohuahub-ai-creator-platform) | AI 创作者社区运营平台 | Dify 4 应用 + RAG + 飞书工作台,周复盘 2h → 3min |
| [飞书办公小助手](https://github.com/cangyuyi/feishu-cli-bot) | 本地常驻飞书 AI 助手 | 23 个 function calling 工具、双身份闭环、零第三方依赖,工程完成度高 |
| [Outbound Copilot](https://github.com/cangyuyi/OutboundCopilot) | 外呼客服话术测试 RPA | 飞书表格 ↔ AI 平台毫秒级联动,热键 <10ms、内存 <30MB,测试提效 300% |
| [求职通关攻略](https://github.com/cangyuyi/china-job-search-playbook) | 中国大陆求职闭环 Skill | 建档 → 搜索 → 网申 → 面试 → 谈薪 → 复盘,全流程可复用 |

---

## 🧭 我的 AI 产品工作流

```text
用户/业务问题
    ↓
场景拆解与需求优先级
    ↓
模型、Prompt、RAG、Agent 方案取舍
    ↓
MVP 工作流 + 人机协同兜底
    ↓
离线评测 / 线上指标 / Bad Case 归因
    ↓
灰度发布、复盘与持续迭代
```

### 我特别重视的 5 个问题

| 问题 | 我的关注点 |
| --- | --- |
| 用户为什么需要 AI? | 是否真的减少决策、创作或操作成本,而不只是"加一个聊天框" |
| AI 方案为什么这样设计? | 模型能力、延迟、成本、稳定性和可解释性的取舍 |
| 效果如何被证明? | 评测集、线上指标、对照基线、Bad Case 与人工抽检 |
| 出错时怎么办? | 置信度、重试、降级、人工接管、回滚与用户反馈 |
| 如何持续产生业务价值? | 转化、留存、复购、毛利、效率和用户满意度 |

---

## 🛠️ 工具与技术

**AI 产品** · Prompt Engineering · Agent Workflow · RAG · 知识库 · LLM 评测 · 多模型选型 · 人机协同

**产品与数据** · 用户访谈 · PRD · 原型 · 指标体系 · Bad Case 归因 · SQL · 项目推进 · 复盘

**开发协作** · Python · TypeScript · Next.js · FastAPI · Go · Docker · PostgreSQL · Redis · LangGraph · LiteLLM · Vibe Coding

**AIGC 工具** · ChatGPT · DeepSeek · Midjourney · 可灵 · 即梦 · Coze · Dify · Codex

---

## 📬 联系我

如果你正在招聘 **AI 产品经理 / AI 应用产品 / Agent 产品 / AI 电商产品**,欢迎通过 GitHub 与我交流。

<p align="center">
  <sub>把 AI 做成产品,而不是只做一个 Demo。</sub>
</p>
