<!-- SVENKUNKKA-README-NAV:BEGIN -->
[English overview](#project-overview-en) · [中文项目说明](#project-overview-zh) · [Maintainer on X / 维护者 X](https://x.com/Svenu1s5)
<!-- SVENKUNKKA-README-NAV:END -->

<!-- SVENKUNKKA-PROJECT-INFO:BEGIN -->

<a id="project-overview-en"></a>
## English project overview

A lightweight adapter that turns Markdown outlines into editable PPTX files, supporting titles, bullets, and notes for quick drafts. The upstream tools listed in the original README offer options for more complex presentations.

**Getting started:** Install `python-pptx`, then run `python scripts/md2pptx.py outline.md -o out.pptx`. Use `# title` for a new slide, `- ` for bullets, and `> ` for notes.

**Scope:** Provides a quick-draft script and `SKILL.md`, rather than a complete template-extraction, visual-design, and review system.

**Repository maintainer / 仓库维护者:** [SvenKunkka](https://github.com/SvenKunkka) · [X / Twitter](https://x.com/Svenu1s5)

<a id="project-overview-zh"></a>
## 中文项目说明

将 Markdown 大纲转换为可编辑 PPTX 的轻量适配层，支持标题、要点和备注，适合快速形成初稿；复杂演示文稿可参考原文列出的上游工具。

**使用入口：** 安装 `python-pptx` 后运行 `python scripts/md2pptx.py outline.md -o out.pptx`；以 `# 标题` 新建页面、`- ` 标记要点、`> ` 标记备注。

**范围说明：** 提供快速出稿脚本与 `SKILL.md`，不等同于完整的模板提取、视觉设计和审查系统。

<!-- SVENKUNKKA-PROJECT-INFO:END -->

---



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


