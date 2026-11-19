
# CNKI论文保真精修 Skill

一个面向知网AIGC检测场景的中文学术论文修改 Skill，主要用于优化论文表达、减少模式化语言，同时最大程度保留原文的核心意思、专业术语、数据和引用。

本 Skill 以用户上传的两份知网AIGC检测报告及连续的矿业工程学术段落改写实践为依据，旨在形成一套可复用的中文学术论文保真精修方法。

## 核心功能

- 学术语言优化：改善句式结构和学术表达，使语言更加自然、准确。
- 降低模式化表达：减少模板化、重复性和过度规整的语言特征。
- 原意保留：不改变原文研究观点、技术逻辑和核心结论。
- 专业信息保真：保留专业术语、数据、单位、图号及参考文献引用。
- 章节针对性修改：根据论文不同章节的写作特点调整修改策略。

## 文件结构

- `SKILL.md`：主技能定义，包含触发条件、工作流程、硬约束、不同章节写作策略和输出要求。
- `references/report-comparison.md`：两份报告对照及证据边界。
- `references/quality-check.md`：术语、数据、图号、引文、限定词核验。
- `examples/mining-rewrite-examples.md`：矿业工程示例。

## 使用方法

将整个 Skill 文件夹放入支持 Agent Skills 的技能目录，或按照对应工具的要求安装。

在对话中输入：

`按 cnki-thesis-fidelity-rewrite 的规则改写下面的论文段落，保持原意、数据和引用，不增加内容：`

然后粘贴需要修改的论文原文。

没有 Skill 功能的对话系统，也可以将 `SKILL.md` 的全部文字放入自定义指令，再发送正文。

## 重要限制

第二次报告检测的是选段汇编，不能与原论文全文的AI特征值直接作涨跌对比。

本 Skill 旨在通过规范化的修改流程改善学术表达质量与原文保真性，不保证知网AIGC检测数值一定下降，也不保证特定检测结果。

## 公开方法参考（非检测原理证明）

- https://github.com/qingshanliuci/cnki-aigc---skill
- https://github.com/xiaofenggan01/aigc-reduce
- https://github.com/imSuYuan/aigc-reducer-skill
