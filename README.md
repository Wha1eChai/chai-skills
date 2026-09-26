# Interface Design Skill

A reusable [Agent Skill](https://agentskills.io/) for designing, building, reviewing, and refining user interfaces with task-aware structure, visual craft, and honest interaction states.

It applies to product UI, dashboards, forms, purchase flows, documentation, marketing pages, creative tools, and project design systems. It supports advice, review, proposals, and implementation without prescribing a framework or a single visual style. Backend-only tasks and unrequested redesigns are outside its scope.

## Install

Clone this repository, then copy `interface-design/` (including `references/`) into your agent's user or project skills directory. For Pi, a user-level installation goes under `~/.agents/skills/interface-design/`; a project-level installation goes under `<project>/.agents/skills/interface-design/`. Start a new session or run `/reload` after installation.

The skill is also available explicitly in Pi as `/skill:interface-design`. Other Agent Skills-compatible tools may use different discovery locations and invocation syntax.

## Contents

- [`interface-design/SKILL.md`](interface-design/SKILL.md) — entry point, deliverable boundaries, and routing by decision trigger.
- [`interface-design/references/`](interface-design/references/) — task/layout, surface/style, visual craft, project design, verification, examples, maintenance, and provenance. Read only what the current decision needs.

The skill is guidance, not a UI component library, test runner, or permission to change unrelated product behavior. It respects the target project's requirements, identity, and existing components. Its maintenance notes include synthetic desk-review scenarios; they are not a measured agent benchmark or user study.

## Example requests

- "Review this checkout form's information hierarchy and error recovery; do not edit files."
- "Design a documentation page using the existing design system, then implement and verify it."
- "Propose a scoped DESIGN.md for this project, distinguishing observed conventions from proposed changes."

## Attribution and license

The guidance is an original synthesis informed by the sources documented in [`provenance.md`](interface-design/references/provenance.md); linked third-party material is not bundled. This repository is released under the [MIT License](LICENSE). If future contributions copy third-party text, code, or assets, check their licenses and preserve required notices first.
