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

Clone [chai-skills](https://github.com/Wha1eChai/chai-skills) and copy this **entire `interface-design/` directory** into an Agent Skills-compatible location, preserving `SKILL.md` and `references/`. For Pi, use `~/.agents/skills/interface-design/` (user) or `<project>/.agents/skills/interface-design/` (project). Start a new Pi session or run `/reload`; call `/skill:interface-design` to select it explicitly. Other agents may use different paths or invocation syntax.

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

克隆 [chai-skills](https://github.com/Wha1eChai/chai-skills)，将**整个 `interface-design/` 目录**复制到支持 Agent Skills 的位置，并保留 `SKILL.md` 与 `references/`。使用 Pi 时，可安装到 `~/.agents/skills/interface-design/`（当前用户）或 `<project>/.agents/skills/interface-design/`（单个项目）。启动新会话或运行 `/reload`；需要明确调用时使用 `/skill:interface-design`。其他 Agent 的安装路径和调用方式可能不同。

示例请求：

- “请审查这个结账表单的信息层级和错误恢复方式，不要改文件。”
- “沿用现有设计系统设计一个文档页面，随后实现并验证。”
- “提出一份有明确范围的 DESIGN.md，区分现状约定和拟议变更。”

### 边界

这个 skill 提供方法，不提供项目事实或额外操作权限；项目需求及已确立的界面约定仍是依据。内含的模拟评审场景不是实测基准或用户研究。仓库不附带 UI 运行时、组件库或第三方素材。许可证见仓库根目录的 [MIT License](../LICENSE)，来源说明见 [provenance notes](references/provenance.md)。
