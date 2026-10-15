# grokbot-ppt-skills
从 Markdown 大纲生成可编辑 PPTX 的轻量适配层。

## 优先复用的上游
- [mpuig/agent-slides](https://github.com/mpuig/agent-slides)（MIT）：完整的模板提取、构建、审查流程，复杂 deck 首选（`uvx --from agent-slides slides ...`）
- [jiandong01/pptx-skills](https://github.com/jiandong01/pptx-skills)（MIT）：Markdown + 模板生成
- [python-pptx](https://github.com/scanny/python-pptx)（MIT）

本仓库只提供 `scripts/md2pptx.py`（零配置快速出稿，标题 / 要点 / 备注）和 `SKILL.md`。

## 用法
```bash
pip install python-pptx
python scripts/md2pptx.py outline.md -o out.pptx
```
大纲格式：`# 标题` 开新页，`- ` 为要点，`> ` 为备注。
