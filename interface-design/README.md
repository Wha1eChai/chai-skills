# Interface Design · 界面设计

[English](#english) · [中文](#中文)

## English

`interface-design` is an [Agent Skill](https://agentskills.io/) for designing, building, reviewing, and refining user interfaces. It connects user tasks and information hierarchy with visual expression, interaction states, and proportionate verification. It does not require a particular framework, visual style, or complete design system.

### When to use it

- Product interfaces, dashboards, forms, checkout flows, documentation, marketing pages, and creative tools.
- UI reviews, design proposals, scoped implementation, and project-level design guidance (`DESIGN.md`, shared tokens, or components).
- Work that requires a choice about structure, style, visual craft, behavior, or state handling—not backend-only work or an unrequested redesign.

The entry point is [`SKILL.md`](SKILL.md). It routes decisions to selected files under [`references/`](references/) instead of requiring every reference for every task. [`provenance.md`](references/provenance.md) explains the sources and limitations of the guidance.

### Install and use

Use the [skills CLI](https://github.com/vercel-labs/skills) to install this skill without manually cloning the repository (Node.js required):

```bash
npx skills add Wha1eChai/chai-skills --skill interface-design
```

Choose a supported agent and install scope when prompted. For a non-interactive, user-level Pi install, use `npx skills add Wha1eChai/chai-skills --skill interface-design -a pi -g -y`. To preview what the repository offers, run `npx skills add Wha1eChai/chai-skills --list` (no install). If you prefer manual installation, copy the **whole `interface-design/` folder**, including `SKILL.md` and `references/`, to `~/.agents/skills/` or `<project>/.agents/skills/` for Pi. Start a new Pi session or run `/reload`; call `/skill:interface-design` to select it explicitly. Other agents may use different paths or invocation syntax.

Example requests:

- "Review this checkout form's information hierarchy and error recovery; do not edit files."
- "Design a documentation page using the existing design system, then implement and verify it."
- "Propose a scoped DESIGN.md that separates observed conventions from proposed changes."

### Boundaries

The skill supplies methods, not project facts or permissions. Project requirements and established UI conventions remain authoritative. Its synthetic review scenarios are guidance checks, not measured benchmarks or user research. No UI runtime, component library, or third-party assets are bundled. See the repository [MIT License](../LICENSE) and [provenance notes](references/provenance.md).

## 中文

`interface-design` 是一个用于设计、实现、审查和优化用户界面的 [Agent Skill](https://agentskills.io/)。它把用户任务与信息层级、视觉表达、交互状态及适度验证联系起来，不预设某个框架、视觉风格或完整设计系统。

### 适用场景

- 产品界面、仪表盘、表单、结账流程、文档页、营销页和创作工具。
- 界面评审、设计方案、限定范围的实现，以及项目级设计约定（如 `DESIGN.md`、共享 token 或组件）。
- 需要判断布局结构、风格、视觉细节、行为或状态的工作；不用于纯后端任务，也不会凭空扩大到未请求的改版。

入口文件是 [`SKILL.md`](SKILL.md)。它按当前决策选择性读取 [`references/`](references/) 下的资料，而不是每次加载全部内容。[`provenance.md`](references/provenance.md) 说明指导原则的来源与证据边界。

### 安装与使用

推荐用 [skills CLI](https://github.com/vercel-labs/skills) 安装，无须手动克隆整个仓库（需要 Node.js）：

```bash
npx skills add Wha1eChai/chai-skills --skill interface-design
```

按提示选择目标 Agent 与安装范围。免交互安装到 Pi 的用户级目录，可用 `npx skills add Wha1eChai/chai-skills --skill interface-design -a pi -g -y`。仅查看仓库中的 skill、暂不安装，可运行 `npx skills add Wha1eChai/chai-skills --list`。若选择手动安装，需将**整个 `interface-design/` 目录**（包括 `SKILL.md` 和 `references/`）复制到 Pi 的 `~/.agents/skills/` 或 `<project>/.agents/skills/`。启动新 Pi 会话或运行 `/reload` 后，可用 `/skill:interface-design` 明确调用。其他 Agent 的安装路径或调用方式可能不同。

示例请求：

- “请审查这个结账表单的信息层级和错误恢复方式，不要改文件。”
- “沿用现有设计系统设计一个文档页面，随后实现并验证。”
- “提出一份有明确范围的 DESIGN.md，区分现状约定和拟议变更。”

### 边界

这个 skill 提供方法，不提供项目事实或额外操作权限；项目需求及已确立的界面约定仍是依据。内含的模拟评审场景不是实测基准或用户研究。仓库不附带 UI 运行时、组件库或第三方素材。许可证见仓库根目录的 [MIT License](../LICENSE)，来源说明见 [provenance notes](references/provenance.md)。
