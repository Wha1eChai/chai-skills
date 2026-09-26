# chai-skills

[English](#english) · [中文](#中文)

## English

A collection of reusable [Agent Skills](https://agentskills.io/) by Wha1eChai. Each skill lives in its own directory with a `SKILL.md`, supporting files, and a bilingual README. The repository currently contains one skill; additional skills can be added independently.

| Skill | Purpose |
| --- | --- |
| [interface-design](interface-design/README.md) | Design, build, review, and refine user interfaces with task-aware structure, visual craft, and honest interaction states. |

### Install

Clone this repository and copy the **skill directory you need** (not the repository root) into a skills location supported by your agent. For Pi, copy `interface-design/` to `~/.agents/skills/interface-design/` for user-level use or `<project>/.agents/skills/interface-design/` for project-level use. Start a new Pi session or run `/reload`, then invoke `/skill:interface-design` if you want to select it explicitly.

Read the [skill README](interface-design/README.md) for scope and examples. This repository is licensed under [MIT](LICENSE). Individual skills retain their provenance notes where relevant.

## 中文

Wha1eChai 的可复用 [Agent Skills](https://agentskills.io/) 集合。每个 skill 独立存放在自己的目录中，包含 `SKILL.md`、配套文件和中英文 README。目前收录一个 skill，后续可以独立增加。

| Skill | 用途 |
| --- | --- |
| [interface-design](interface-design/README.md) | 围绕任务结构、视觉表现和真实交互状态，设计、实现、审查与优化用户界面。 |

### 安装

克隆仓库后，将**所需的 skill 目录**（而不是整个仓库根目录）复制到 Agent 支持的 skills 路径。使用 Pi 时，可将 `interface-design/` 复制到 `~/.agents/skills/interface-design/` 供当前用户使用，或放在 `<project>/.agents/skills/interface-design/` 供单个项目使用。启动新的 Pi 会话或运行 `/reload`；需要明确调用时使用 `/skill:interface-design`。

适用范围与示例请参阅 [skill README](interface-design/README.md)。本仓库采用 [MIT 许可证](LICENSE)；各 skill 的来源说明保存在对应目录中。
