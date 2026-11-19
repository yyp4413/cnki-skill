# CNKI论文保真精修 Skill

这是一个可复用的 Markdown Skill，以用户上传的两份知网AIGC检测报告及连续的矿业工程学术段落改写实践为依据。

## 文件

- `SKILL.md`：主技能定义（包含触发条件、工作流程、硬约束、不同章节写作策略和输出要求）。
- `references/report-comparison.md`：两份报告对照及证据边界。
- `references/quality-check.md`：术语、数据、图号、引文、限定词核验。
- `examples/mining-rewrite-examples.md`：矿业工程示例。

## 使用

- 将整个文件夹放入支持 SKILL.md 的技能目录，或直接将 `SKILL.md` 复制到已有技能目录。
- 在对话中输入：`按 cnki-thesis-fidelity-rewrite 的规则改写下面的论文段落，保持原意、数据和引用，不增加内容：`，再粘贴原文。
- 没有技能功能的对话系统，也可以将 `SKILL.md` 的全部文字放入自定义指令，再发送正文。

**重要限制**：第二次报告检测的是选段汇编，不能与原论文全文的AI特征值直接作涨跌对比。Skill 只保证按规则努力提高学术表达质量与保真性，不保证知网AIGC数值变化。

## 公开方法参考（非检测原理证明）

- https://github.com/qingshanliuci/cnki-aigc---skill
- https://github.com/xiaofenggan01/aigc-reduce
- https://github.com/imSuYuan/aigc-reducer-skill
