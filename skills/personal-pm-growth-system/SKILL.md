---
name: personal-pm-growth-system
description: "Operate the personal product capability and interview growth system: route preparation, interview review, improvement actions, and asset updates across its Feishu docs and Bases while preserving evidence boundaries. Use for this personal system, not for ordinary standalone interview or PRD requests."
---

# 个人产品能力与面试成长系统

协调个人系统中的资料读取、专业分析、资产更新提案与验证；不替代已有的面试、PRD、评审或 AI 专项 Skill。

## 适用边界

仅在用户明确要使用、维护或复盘这套「个人产品能力与面试成长系统」时使用。普通的单题面试回答、独立 PRD 撰写或一次性案例练习，直接使用相应专业 Skill，不要为了建立记录而强行纳入系统。

## 先读什么

每次先读取 [`references/system-map.md`](references/system-map.md)，根据当前任务只读取其中指向的必要文档或 Base 表。涉及新增、修改或关联任一资产时，再读取 [`references/update-gate.md`](references/update-gate.md)。

涉及本系统本地控制文档或本 Skill 的已确认写入时，再读取 [`references/github-sync.md`](references/github-sync.md)。该参考仅规定受控同步到 GitHub 的条件与边界，不授权其他本地资料进入仓库。

不要凭记忆使用表 ID、字段选项或目录层级；写入前读取目标表当前 schema 和目标文档当前正文。系统地图只提供入口和对象职责，不取代实时核验。

## 工作模式

根据用户意图选择一个或多个模式，并说明本轮会读取的资产与是否会写入：

1. **岗位准备**：从 JD、岗位准备包或目标方向出发，定位相关母题、项目证据、项目上下文、SOP 与能力短板；再按需要使用 `ai-pm-interview-prep`、`interview-self-introduce`、`ai-pm-evaluation-lab` 或 `ai-pm-cost-model-selection` 的专业规则。
2. **面试记录与复盘**：建立或读取“岗位父文档 → 场次父文档 → 原始记录／复盘”资料；区分整场结论、单题原始问答、面试官直接反馈、复盘推断与待验证建议。需要模拟练习时使用 `ai-pm-case-interviewer`。
3. **改进与验证**：把值得处理的缺口转化为具体行动，或关联到长期能力主题；区分口头表达练习、项目证据补全、工作方式改进、方法论／SOP 更新和暂不可执行的建议。
4. **资产更新提案**：判断某项信息应更新母题与答案、项目上下文、可复用项目证据、需求生命周期资料、SOP／模板，还是只保留在原始记录；先提交最小更新提案。
5. **一致性检查**：只读检查链接、状态、事实来源、同义题、重复正文、行动闭环和验证证据；输出问题与建议，不自动修复。

## 核心约束

- 先判断对象边界：母题、答案、真实问题、完整原始记录、复盘、项目证据、SOP、行动和能力主题不能因名称相近而合并正文。
- 使用四类标记：**已确认事实**、**面试官直接反馈**、**复盘推断**、**建议／待验证**。不得把后两类写成事实，也不得把行动完成写成能力改善。
- 真实问题默认完整留存；只有具有复用价值、明确缺口或需要后续处理时，才进入“实际问题与复盘”结构化管理。
- 高价值需求的完整生命周期资料优先留在项目资料目录；系统只管理筛选、价值、入口、状态及必要的个人反思，不复制整套 PRD／上线材料。
- 既有专业 Skills 负责其专业判断。本 Skill 只负责选择正确输入、承接输出到正确资产，并阻止未经授权的跨资产写入。
- 单次面试、单条反馈或一次练习不能直接改写全局 SOP、能力结论或通用母题规则；先保留为候选，并按证据强度决定是否提出升级建议。

## 通用流程

1. 明确任务模式、目标、时间范围和是否允许写入；读取最小必要上下文。
2. 输出对象清单：已读来源、证据状态、当前缺口，以及准备调用的专业 Skill（如有）。
3. 给出结果或复盘，并指出每个结论属于哪一类证据。
4. 如发现可沉淀内容，给出“目标资产、拟写入内容、不会改动什么、风险”的最小更新提案。
5. 只有用户明确确认该写入范围后，才创建、编辑或关联文档／Base 记录；写后回读目标正文、字段与关联并对照验收条件。
6. 若变更会新增／删除核心表、字段、目录层级、Skill 或改变既有对象职责，停止写入，提交架构变更提案。
7. 若本轮产生已确认且已验证的本地系统变更，按 Git 同步参考完成受限范围的提交与推送；任何范围外改动、冲突或认证异常都停止并报告，不自行处理。

## 输出要求

默认先交付可执行结论，随后用紧凑列表列出：已用证据、未验证项、建议更新的资产、是否需要用户确认。只在用户授权的范围内写入，不把“生成草案”说成“已写入飞书”。

## 路由提示

- 准备岗位或组织题库：`ai-pm-interview-prep`
- 自我介绍：`interview-self-introduce`
- 压力／案例模拟：`ai-pm-case-interviewer`
- AI 产品评估、Bad Case、发布质量：`ai-pm-evaluation-lab`
- 模型成本或模型选择：`ai-pm-cost-model-selection`
- 项目内部需求资料、PRD、需求审查：`pm-project-memory`、`pm-requirement-writer`、`pm-review`
- 稳定的工作方法反馈是否应进入 Skill：`pm-skill-evolution`
- 飞书正文、知识库层级与 Base 操作：`lark-doc`、`lark-wiki`、`lark-base`
