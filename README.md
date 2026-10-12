# 王泽栋 · AI 产品 / AI 应用 / Agent

2027 届 · 浙江农林大学智慧农业本科 · 杭州。求职方向：**AI 产品经理、AI 应用 / Agent、AI 电商产品**。

我关注的不是“能否生成一个答案”，而是**需求判断 → 工作流设计 → 可追溯评测 → 风险兜底 → 复盘迭代**。这里既有业务实践，也有独立开发的工程原型；二者的证据和可复现范围不同，下面分别说明。

## 先看三项代表作

| 项目 | 我的工作与适用场景 | 现在能核查什么 / 不能证明什么 |
| --- | --- | --- |
| **[Mago AIGC Platform](https://github.com/cangyuyi/Mago-AIGC-Platform)** | AIGC 创意生产平台相关产品实践：多模型聚合、Agent 工作台、从需求到工作流设计 | [公开实现与架构](https://github.com/cangyuyi/Mago-AIGC-Platform#readme)。公开代码**不等于**线上生产系统；历史业务成果需单独核对统计口径。 |
| **[crop-guard-agent](https://github.com/cangyuyi/crop-guard-agent)** | 独立工程原型：在作物用药合规案例中，将可判定规则和模型建议分离 | `python3 -m unittest discover -s tests`：40 项测试；[在线演示](https://cangyuyi.github.io/crop-guard-agent/docs/)；安全门禁只在仓库给定数据与测试范围内验证，不能推广为真实农事或跨行业零风险。 |
| **[invoice-risk-review-agent](https://github.com/cangyuyi/invoice-risk-review-agent)** | 独立票据风险审核原型：字段提取、确定性规则、证据链和人工接管 | `python3 eval/evaluate.py`：36/36 项**合成结构化数据规则回归**；[静态交互演示](https://cangyuyi.github.io/invoice-risk-review-agent/)；不等同于 OCR 准确率或真实税务/审批结果。 |

**阅读顺序**：招聘方先看 Mago 的产品决策与职责，再看 crop-guard 的规则/评测门禁，最后看 invoice 的人机协作与证据链。所有演示以各仓库 README 的实际前置条件为准。

## 业务实践与独立复现

| 项目 | 性质与核查边界 |
| --- | --- |
| [HuohuaHub](https://github.com/cangyuyi/huohuahub-ai-creator-platform) | AI 创作者平台相关业务案例。仓库公开部分 AI 日报代码、Dify DSL 与**静态交互示意**；其他线上业务模块、使用人数和效率数字是个人业务陈述，不是该仓库可复跑的结果。 |
| [电视选购 Copilot](https://github.com/cangyuyi/tv-buying-copilot) | 电商导购场景的**独立重做原型**，不是原公司内部系统。`python3 eval.py` 检查 25 条当前实现的确定性冒烟用例；历史人工质量评分缺逐例打分，**不将 72%→92% 写作可复核结论**。 |

## 工具与方法作品

| 项目 | 看点与边界 |
| --- | --- |
| [飞书 CLI 助手](https://github.com/cangyuyi/feishu-cli-bot) | 本地工具调用与安全开关；`PYTHONPATH=src python3 -m unittest discover -s tests`：36 项。Python 标准库运行时不代表免装 `lark-cli`、无需授权或模型服务。 |
| [商策 Agent](https://github.com/cangyuyi/shance-commerce-agent-portfolio) | 电商内容评测框架；当前 Benchmark 结果是预置演示数据，不是已实测的 LLM 成绩。 |
| [瑞幸用户运营 Agent](https://github.com/cangyuyi/lucky-growth-agent) | 竞赛命题下的 Dify DSL 原型，**不代表品牌方官方上线**。 |
| [MSDS 危害识别](https://github.com/cangyuyi/msds-hazard-agent) | 实习后独立重做的 OCR / CAS 辅助识别案例；知识表未命中不等于无危害，专业结论需人工复核。 |
| [Outbound Copilot](https://github.com/cangyuyi/OutboundCopilot) | 飞书表格到对话平台的话术测试 RPA；部署环境与时间收益需现场验证。 |
| [网申人机协作 SOP](https://github.com/cangyuyi/campus-apply-copilot) | 专注 ATS 填表和登录、提交交接；投递数量是个人自述，不是仓库可自动验证指标。 |
| [求职通关攻略](https://github.com/cangyuyi/china-job-search-playbook) | 全程岗位核验、材料、面试与 Offer 流程；网申专项见上一项。 |
| [AI PM 简历写作 Skill](https://github.com/cangyuyi/ai-pm-sop) | 证据优先的简历诊断与改写 SOP；不替用户编造经历。 |

## 工程探索与社区

- [长夜收割者](https://github.com/cangyuyi/midnight-survivors)：浏览器游戏工程练习；**目前未指定开源许可证**。
- [黎明幸存者](https://github.com/cangyuyi/dawn-survivors)：早期**构建产物展示**，仓库不含可供审查的源代码。
- [BossHunter](https://github.com/cangyuyi/BossHunter)：社区项目的 **fork**，不列作本人原创项目；如需了解贡献，应以可核实的 PR / 提交为准。

## 联系

如有 AI 产品 / Agent / AI 电商岗位交流机会，可通过 [GitHub Issue](https://github.com/cangyuyi/cangyuyi/issues) 联系，或邮件至 **wangzedong2027@foxmail.com**。具体业务指标与职责范围以面谈时可合规提供的材料为准。
