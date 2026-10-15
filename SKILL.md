---
name: pptx-from-outline
description: 需要把大纲、报告或会议内容做成可编辑 PPT 时使用；简单稿用 md2pptx.py，复杂稿用上游 agent-slides。
---
# 步骤
1. 明确受众、页数、结论先行的标题。
2. 写 Markdown 大纲（# 页标题 / - 要点 / > 备注），每页不超过 5 个要点。
3. 简单稿：`python scripts/md2pptx.py outline.md -o deck.pptx`；有品牌模板或图表需求：用 agent-slides。
4. 用 LibreOffice 渲染成图片逐页检查溢出、错字。
5. 交付 PPTX 和一句话改动说明。
