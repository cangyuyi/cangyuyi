# 王泽栋 · AI 产品经理

**AI 应用 / Agent / AI 电商 · 从 0 到 1 落地，评测驱动，结果导向**

浙江农林大学 · 智慧农业本科生（2023.09–2027.06）· 杭州 · 2027 届校招

> **我关注的问题：如何把大模型能力变成可用、可评测、可持续迭代，并且真正服务业务结果的产品。**

<p align="center">
  <img src="https://img.shields.io/badge/%E5%85%AC%E5%BC%80%E4%BB%93%E5%BA%93-16-24292f" alt="公开仓库">
  <img src="https://img.shields.io/badge/%E5%9C%A8%E7%BA%BF%20Demo-3%20%E4%B8%AA%C2%B7%E7%82%B9%E5%BC%80%E5%8D%B3%E7%94%A8-2ea44f" alt="在线 Demo">
  <img src="https://img.shields.io/badge/%E5%8F%AF%E5%A4%8D%E7%8E%B0%E8%AF%84%E6%B5%8B-36%2F36%20%E8%A7%84%E5%88%99%E5%9B%9E%E5%BD%92-6f42c1" alt="可复现评测">
  <img src="https://img.shields.io/badge/%E9%9B%B6%E7%AC%AC%E4%B8%89%E6%96%B9%E4%BE%9D%E8%B5%96-clone%20%E5%8D%B3%E8%B7%91-0052cc" alt="零第三方依赖">
</p>

---

## 🔍 先看这三个：点开就能验证

不用 clone、不用配置、不用先相信我的形容词。

| 入口 | 是什么 | 值得看的点 |
| --- | --- | --- |
| **[在线 Demo →](https://cangyuyi.github.io/invoice-risk-review-agent/)** | 企业报销票据风险审核工作流 | 高风险场景下 AI 工作流该怎么设计：确定性规则 + 三路字段提取 + 证据链 + 人工兜底，**自动放行率固定 0%** |
| **[在线试玩 →](https://cangyuyi.github.io/midnight-survivors/)** | 浏览器 Roguelite《长夜收割者》 | 数据导向工程：SoA 定长对象池、空间哈希网格、60 Hz 固定步长模拟，稳态**零堆分配**；零外部美术与音频资源 |
| **[clone 即跑 →](https://github.com/cangyuyi/feishu-cli-bot)** | 本地常驻飞书 AI 助手 | **23 个 function calling 工具**、零第三方依赖、36 个测试 + CI 覆盖 Python 3.9–3.13 |

> 说明：主页中的业务数据已做去标识、区间化或相对化处理，面试时可在合适的保密边界内展开具体口径。下面标注为「开源作品」的项目均可独立克隆、运行与复核。

---

## 🏆 开源作品（可复核）

### 1. [Mago AIGC Platform](https://github.com/cangyuyi/Mago-AIGC-Platform) — 聚合型 AIGC 内容生产平台 · 产品负责人

> 多模型聚合 + 场景化封装 + 多 Agent 协作 · 从 0 到 1 · **生产环境连续盈利**

**结果**：第 3 个月首次单月盈利、6 个月实现连续正向盈利；峰值日生成 20 万+ 张，日均 8–12 万张；单位算力成本比单一官方渠道低 38%；99.9% 企业级可用性；付费企业月复购 75%+；LTV/CAC > 7；综合毛利率 25%–30%。

**我做了什么**：

- 深度访谈创作者与企业客户，提炼 API 不稳定、并发卡顿、场景脱节等关键痛点
- 规划绘图、视频、画布、电商、素材库五大模块，负责电商场景与前端产品落地
- 设计"热点情报 → 创意发散 → 脚本创作 → 角色/风格 → 提示词生成 → 一键生成"产品闭环
- 设计 8 个 Agent 协作的脚本工作流，沉淀 Prompt 模板、知识库与人工确认机制
- 用模型选型、Prompt 迭代、重试/反馈/阈值/归因/修复，平衡效果、稳定性与成本

**工程规模**（可在仓库核对）：约 1.3 万行 Python + 5,300 行 Go + 7,300 行 TypeScript；21 节点 LangGraph 状态机与 4 个人工确认闸口；29 个测试文件；CI 含真 Postgres 的全栈浏览器 E2E。

**面试可展开**：用户研究、MVP 取舍、模型路由、工作流编排、容错设计、可观测性、定价与毛利。

<p align="center">
  <img src="https://raw.githubusercontent.com/cangyuyi/Mago-AIGC-Platform/main/screenshots/03-mago-canvas-workflow.png" alt="Mago 工作流画布" width="48%" />
  <img src="https://raw.githubusercontent.com/cangyuyi/Mago-AIGC-Platform/main/screenshots/04-mago-ecommerce-workstation.png" alt="Mago 电商工作台" width="48%" />
</p>

📌 [产品 README](https://github.com/cangyuyi/Mago-AIGC-Platform#readme) · [用户研究](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/01-user-research-summary.md) · [Prompt 迭代 SOP](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/02-prompt-iteration-sop.md) · [容错与降级](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/03-error-handling-mechanism.md) · [定价与毛利](https://github.com/cangyuyi/Mago-AIGC-Platform/blob/main/docs/04-pricing-and-margin.md)

---

### 2. [电视选购 Copilot](https://github.com/cangyuyi/tv-buying-copilot) — 纯 Python 自研 Multi-Agent 导购系统 · 独立原型

> 从零自研的电商导购 Agent 全流程独立重做版 · 含 PRD、评测集、MCP

**结果**：25 条评测集驱动一轮迭代，通过率 **V1.0 72% → V1.1 92%**，异常输入零崩溃。

- 四层架构：Master Router + 5 个 Skill Worker + Replanner + Compliance，高风险售后强制转人工
- 内置 MCP 工具服务（商品检索 / 促销计算 / 履约查询 / 售后政策），**零第三方依赖，clone 即跑**
- 评测集、逐条评测记录与评分口径全部入库，可自行复核

📌 [AI_PRD](https://github.com/cangyuyi/tv-buying-copilot/blob/main/AI_PRD.md) · [V1.0 评测报告](https://github.com/cangyuyi/tv-buying-copilot/blob/main/evaluation/eval-results-v1.md) · [V1.1 评测报告](https://github.com/cangyuyi/tv-buying-copilot/blob/main/evaluation/eval-results-v1.1.md)

---

### 3. [报销票据风险审核 Agent](https://github.com/cangyuyi/invoice-risk-review-agent) — 企业报销风险审核原型

> 高风险场景的 AI 工作流：宁可转人工，不可错放行

**结果**：36 条确定性规则回归 **36/36 通过**（可复现）；二维码 / OCR / 视觉三路字段提取并附基线与逐例结果；**自动放行率固定 0%**，全部结论带规则证据并可记录人工复核。

- 在线 Demo 与 `demo/` 源码同源，使用仓库内合成数据，不连接税务平台、不执行真实审批
- 评测脚本与逐例结果入库，`python eval/evaluate.py` 可直接复跑

📌 [在线 Demo](https://cangyuyi.github.io/invoice-risk-review-agent/) · [仓库 README](https://github.com/cangyuyi/invoice-risk-review-agent#readme)

---

### 4. [飞书办公小助手](https://github.com/cangyuyi/feishu-cli-bot) — 本地常驻飞书 AI 助手

> 复用本机 lark-cli + 任意 OpenAI 兼容大模型，无需开放平台后台配置

- **23 个 function calling 工具**，工具表与实现由测试断言保持一致
- **零第三方运行时依赖**（仅标准库），36 个单元测试通过，CI 覆盖 Python 3.9–3.13
- 含 10 项工程加固记录（HARDENING.md），明确标注未完成的权限与确认项

📌 [仓库 README](https://github.com/cangyuyi/feishu-cli-bot#readme) · [工程加固记录](https://github.com/cangyuyi/feishu-cli-bot/blob/main/HARDENING.md)

---

### 5. [campus-apply-copilot](https://github.com/cangyuyi/campus-apply-copilot) — 校招网申人机协作 SOP

> 把"投递"这件重复劳动产品化为可复用、可校验、可止损的流程

- 五类 ATS 平台（北森 / 摩卡 / 飞书招聘 / 牛客 / 智联）的差异化解法与降级阶梯
- 校验驱动法：提交前断言校验，宁可暂停不可错填；含一次真实数据事故的完整复盘
- 附可运行工具脚本（中文 PDF 生成、流程追踪、脱敏自检），全部经过实际投递验证

📌 [仓库 README](https://github.com/cangyuyi/campus-apply-copilot#readme)

---

## 💼 工作案例（业务数据已脱敏）

### 头部电商平台 AI 导购 Agent · 知识库 / Prompt / 评测闭环

> 面向真实电商咨询场景的 AI 产品迭代案例 · **评测驱动，效果可证明**

**结果**：脱敏后商品匹配准确率提升约 **15 个百分点**，参数类 Bad Case **下降约六成**，满意度明显提升；咨询转化与 AI 自主解决率提升，人工转接率明显下降。

**我做了什么**：

- 重构商品知识库：四类知识分库、标签体系、切片策略、SLA 与六步更新 SOP
- 设计 6 套导购 Prompt 模板，建立版本管理与离线评测机制
- 搭建转化率、人工转接率、响应时长、满意度等全维度指标看板
- 用"表现层 → 策略层 → 数据层 → 模型层"四层方法定位 Bad Case，按优先级推动修复

**面试可展开**：为什么先修知识库而不是先调模型、如何建立评测集、如何证明指标提升、如何处理大促风险。

> 该项目为公司内部系统，仓库不公开；上面的电视选购 Copilot 是我对其全流程的独立重做版，代码与方法论可公开复核。

---

## 🧪 更多作品

| 项目 | 一句话 | 亮点 |
| --- | --- | --- |
| [商策 Agent](https://github.com/cangyuyi/shance-commerce-agent-portfolio) | 电商营销内容 Agent 作品集 | 20 例 Benchmark，同一套评测对比单次 Prompt / 结构化 Prompt / Agent 工作流 |
| [瑞幸用户运营 Agent](https://github.com/cangyuyi/lucky-growth-agent) | 2026 AI 先锋大赛 · 瑞幸命题 | 意图识别 + 生命周期策略 + 置信度分级，DSL 可自部署 |
| [MSDS 职业危害识别](https://github.com/cangyuyi/msds-hazard-agent) | 职业卫生辅助识别原型 | PDF/OCR 成分提取 + CAS 校验位校验 + 知识表匹配 + 人工复核，V1→V2 三轮迭代 |
| [火花工坊 HUB](https://github.com/cangyuyi/huohuahub-ai-creator-platform) | AI 创作者社区运营平台 | Dify 应用 + RAG 问答 + 飞书工作台，周复盘 2h → 3min |
| [Outbound Copilot](https://github.com/cangyuyi/OutboundCopilot) | 外呼话术测试自动化 | 飞书表格 ↔ 对话平台联动，鼠标侧键一键跳转粘贴；含 Chrome 扩展 + 跨平台热键三端实现 |
| [长夜收割者](https://github.com/cangyuyi/midnight-survivors) | 浏览器 Roguelite（可在线试玩） | TypeScript 自研引擎：固定步长模拟 + 空间哈希 + 定长对象池，CI / Pages 全绿 |
| [黎明幸存者](https://github.com/cangyuyi/dawn-survivors) | 浏览器幸存者 Roguelite | 同系列早期版本，在线可玩 |
| [求职通关攻略](https://github.com/cangyuyi/china-job-search-playbook) | 中国大陆求职闭环 Skill | 建档 → 搜索 → 网申 → 面试 → 谈薪 → 复盘，含 4 个可运行脚本 |
| [AI PM Resume Skill](https://github.com/cangyuyi/ai-pm-sop) | AI 产品经理简历诊断与改写 | 七维诊断框架 + STAR/XYZ 改写 + 三类岗位差异化输出 |

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
| 用户为什么需要 AI？ | 是否真的减少决策、创作或操作成本，而不只是"加一个聊天框" |
| AI 方案为什么这样设计？ | 模型能力、延迟、成本、稳定性和可解释性的取舍 |
| 效果如何被证明？ | 评测集、线上指标、对照基线、Bad Case 与人工抽检 |
| 出错时怎么办？ | 置信度、重试、降级、人工接管、回滚与用户反馈 |
| 如何持续产生业务价值？ | 转化、留存、复购、毛利、效率和用户满意度 |

---

## 🛠️ 工具与技术

**AI 产品** · Prompt Engineering · Agent Workflow · RAG · 知识库 · LLM 评测 · 多模型选型 · 人机协同

**产品与数据** · 用户访谈 · PRD · 原型 · 指标体系 · Bad Case 归因 · SQL · 项目推进 · 复盘

**开发协作** · Python · TypeScript · Next.js · FastAPI · Go · Docker · PostgreSQL · Redis · LangGraph · LiteLLM

**AIGC 工具** · ChatGPT · DeepSeek · Midjourney · 可灵 · 即梦 · Coze · Dify · Codex

---

## 📬 联系我

如果你正在招聘 **AI 产品经理 / AI 应用产品 / Agent 产品 / AI 电商产品**，欢迎联系：

- 📮 邮箱：**wangzedong2027@foxmail.com**
- 💬 也可以直接开 Issue 或通过 GitHub 与我交流

<p align="center">
  <sub>把 AI 做成产品，而不是只做一个 Demo。</sub>
</p>
