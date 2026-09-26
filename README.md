# chai-skills

[English](#english) · [中文](#中文)

## English

A collection of reusable [Agent Skills](https://agentskills.io/) by Wha1eChai. Each skill lives in its own directory with a `SKILL.md`, supporting files, and a bilingual README. The repository currently contains one skill; additional skills can be added independently.

| Skill | Purpose |
| --- | --- |
| [interface-design](interface-design/README.md) | Design, build, review, and refine user interfaces with task-aware structure, visual craft, and honest interaction states. |

### Install

Install only the skill you want with the [skills CLI](https://github.com/vercel-labs/skills) (Node.js required):

```bash
npx skills add Wha1eChai/chai-skills --skill interface-design
```

The CLI lets you choose a supported agent and install scope. To install this skill globally for Pi without prompts:

```bash
npx skills add Wha1eChai/chai-skills --skill interface-design -a pi -g -y
```

Use `npx skills add Wha1eChai/chai-skills --list` to inspect the available skills without installing. Alternatively, manually copy the entire `interface-design/` directory to Pi's `~/.agents/skills/` or a project's `.agents/skills/`. Start a new Pi session or run `/reload`; use `/skill:interface-design` to invoke it explicitly.

Read the [skill README](interface-design/README.md) for scope and examples. This repository is licensed under [MIT](LICENSE). Individual skills retain their provenance notes where relevant.

## 中文

Wha1eChai 的可复用 [Agent Skills](https://agentskills.io/) 集合。每个 skill 独立存放在自己的目录中，包含 `SKILL.md`、配套文件和中英文 README。目前收录一个 skill，后续可以独立增加。

| Skill | 用途 |
| --- | --- |
| [interface-design](interface-design/README.md) | 围绕任务结构、视觉表现和真实交互状态，设计、实现、审查与优化用户界面。 |

### 安装

推荐使用 [skills CLI](https://github.com/vercel-labs/skills) 按需安装单个 skill（需要 Node.js）：

```bash
npx skills add Wha1eChai/chai-skills --skill interface-design
```

CLI 可选择目标 Agent 和安装范围。为 Pi 免交互安装到用户级目录：

```bash
npx skills add Wha1eChai/chai-skills --skill interface-design -a pi -g -y
```

想先查看可安装内容、暂不安装，可运行 `npx skills add Wha1eChai/chai-skills --list`。不使用 CLI 时，也可手动将整个 `interface-design/` 目录复制到 Pi 的 `~/.agents/skills/` 或项目的 `.agents/skills/`。启动新 Pi 会话或运行 `/reload` 后，可用 `/skill:interface-design` 明确调用。

适用范围与示例请参阅 [skill README](interface-design/README.md)。本仓库采用 [MIT 许可证](LICENSE)；各 skill 的来源说明保存在对应目录中。
