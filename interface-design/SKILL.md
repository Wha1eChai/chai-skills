---
name: interface-design
description: Design, build, review, or refine user interfaces with task-aware structure, visual craft, and complete interaction states. Use for product UI, dashboards, forms, purchase flows, documentation, marketing pages, creative tools, or project-level design systems and DESIGN.md. Covers advice, reviews, proposals, and implementation without forcing a visual style or stack. Skip backend-only work, mechanical use of an approved UI pattern, and unrequested redesigns.
---

# Intentional Interface Design

Design interfaces that are easy to read, make important content stand out, and have visual appeal. Help people recognize content effortlessly, understand its structure quickly, and naturally notice information and actions relevant to their task. Use typography, color, proportion, space, imagery, and motion to create a coherent, recognizable expression that invites reading, action, or exploration. Choose and develop that expression from the page's purpose, content, and user preferences. Keep behavior and claims honest.

This skill supplies methods, not project facts. Read relevant project guidance; do not embed account rules, prices, routes, or current defects into the skill. Missing analytics, research, screenshots, or DESIGN.md does not automatically block work.

## 1. Select the deliverable before selecting references

Infer the requested outcome and edit authority from the user's words and project instructions. Do not make the user select an internal mode.

| Request | Deliverable and stopping point | Route |
| --- | --- | --- |
| Discuss, compare, or reason about a design | Recommendation, rationale, tradeoffs, assumptions; no files unless requested | Load only references matching unresolved decisions |
| Assess, audit, or review | Prioritized evidence-backed findings; no implicit fixes | Read Verification before inspection; add decision references by review scope |
| Design a component/page without asking for implementation | Structure, hierarchy, behavior/state specification, and visual direction; specimen when useful | Read matching decision references; Verification for acceptance criteria |
| Build, fix, or implement UI | Working scoped component/page/flow plus relevant verification | Read matching decision references before affected decisions; Verification before meaningful behavior changes |
| Establish/evolve a project's design standard, DESIGN.md, shared tokens, or component system | Scoped project baseline or system change, with explicit status and adoption boundaries | Read Project design first, then its routed references |
| Maintain this skill or analyze upstream guidance | Transferable rule/routing updates and checks | Read Maintenance and Provenance |

A local edit with an established answer may need no additional reference. A request to "design a page" may mean a proposal or working code: use the conversation context; ask one focused question only if this ambiguity materially changes edit authority or the deliverable. A preview component is not automatically production integration.

For combined requests, sequence the requested outputs: proposal → approved/authorized implementation → verification. Do not force a new approval between steps already authorized. Do not stop at a plan when implementation was requested, or proceed to implementation when only advice was requested.

## 2. Read by decision trigger, at the point of need

Inspect the target, nearby implementation, existing components/tokens, and relevant product/design guidance first. Do not audit the whole repository for a local change.

| Reference | Read when | Read before | Skip when |
| --- | --- | --- | --- |
| [Task and layout](references/task-and-layout.md) | Task order, navigation, grouping, layout structure, purchase consequences, forms, async/cross-page continuity are being decided or reviewed | Structure/behavior choices; tests for those behaviors | Applying an established cosmetic change without structural decisions |
| [Surface and style](references/surfaces-and-style.md) | Visual direction, brand continuity, cross-surface differences, or conflicting visual baselines need judgment | Choosing or changing expression | Existing direction is clear and preserved; layout changes alone do not trigger it |
| [Taste and craft](references/taste-and-craft.md) | Actively choosing composition, type, density, color, detail, or motion; reviewing visual quality | Visual implementation or critique | Mechanically applying an approved component/token with no new visual judgment |
| [Positive examples](references/positive-examples.md) | A composition/expression benefits from concrete reference or plausible alternatives need comparison | Developing the relevant choice; start with a useful case and adapt its reasoning | Mechanical edits or a settled choice needing no further exploration |
| [Verification](references/verification.md) | Meaningful behavior/responsive/theme/focus/motion changes, new surface delivery, or review | Selecting states/evidence and implementing; return to selected checks at completion | Tiny known fix with obvious focused checks already covered by the project |
| [Project design](references/project-design.md) | Establishing a project baseline, documenting design, evolving shared tokens/components, or consolidating design drift | Choosing authority, artifact scope, or changing shared values | One-off page/variant work using the established system |
| [Maintenance](references/maintenance.md) / [Provenance](references/provenance.md) | Changing this skill, promoting lessons, or checking sources | Rule changes | Ordinary product design or implementation |

Read a whole short reference when entering a broad unfamiliar decision area; read the named relevant sections for a narrow issue. Load combinations as the union of actual triggers, not a fixed bundle. Reuse context already read; reread only after material updates, scope changes, or lost context. Do not narrate routine document loading.

Typical combinations:
- Known token substitution: entry + project context only.
- Visual card polish: Taste; add Verification for non-trivial state/responsive changes.
- Login recovery: Task + Verification, not Style by default.
- New page in an existing design system: Task + Taste + Verification as decisions require; no automatic Style.
- New brand surface from brief to code: Task + Style + Taste + Verification, loaded in that order of need.
- Project design baseline: Project design → Style + Taste; Task for structural conventions; Verification to define adoption evidence.

## 3. Establish only the context the task needs

Identify a compact working brief: who acts, what must they accomplish, what decision comes next, what information supports it, and what identity/behavior/technical constraints apply. Keep it internal or brief unless it is the requested deliverable.

Approved requirements describe intended behavior; source describes observed behavior. Conflicts remain explicit. Existing implementation does not silently override a requirement, and an old screenshot does not mandate rollback.

For refinement, preserve established identity and behavior while improving the requested experience. Identify the anchors that carry recognition—such as a logo, color family, type character, or interaction vocabulary—and which expressive properties remain open. Within the authorized scope, adjusting lightness, saturation, scale, or rhythm can strengthen the same identity. Explicitly approved values remain constraints until a change is agreed. Missing DESIGN.md does not make an existing product a blank canvas.

Infer low-risk details and proceed with labeled assumptions where needed. Ask only when alternatives materially change the task, cost, permissions, irreversible effects, or costly-to-reverse direction. Block only the affected decision; continue independent work. Never invent business promises, capabilities, proof, or user research.

## 4. Connect task, structure, expression, and implementation

Classify the surface by its dominant user purpose: **Operate** (complete a task), **Read** (understand/find information), **Decide** (evaluate and choose), or **Experience** (inspect/experience an artifact). Mixed regions are allowed; do not assign one skin to an entire company.

Start with what leads, what must be compared or edited together, and the information each decision needs. Develop structure and expression together: real text, imagery, color, and scale can reveal a better composition. Use proportion, proximity, alignment, and contrast to make the relationships clear and the experience engaging.

Give important regions a discoverable visual presence and supporting content comfortable readability. A monitoring screen can make several concurrent signals distinct; a reading page can combine clear wayfinding with a memorable typographic voice. Familiar controls and expressive presentation can work together.

Build with existing components, supported variants, native semantics, and established accessible primitives. Follow the project's framework and styling conventions. This skill grants no dependency installation, production, payment, publication, or broader redesign authority.

Use semantic tokens where available. Introduce small local scales when needed; do not require a full token migration. Route shared token changes through Project design before changing their consumers. Shared semantics can have different theme values; visual consistency does not require merged account domains or frameworks.

## 5. Verify the requested artifact, not an imagined larger delivery

- Advice/proposal: check coherence, alternatives, assumptions, and actionable next steps; no implementation claim.
- UI implementation: check task behavior, visual craft, and code separately.
- Project baseline: check authority, specificity, references, status, and adoption plan; documents are not rollout.
- Token/component change: verify mappings, affected consumers/themes/states, and focused regression evidence.

Use realistic content shapes and label synthetic examples. Do not fabricate prices, testimonials, progress, health, or successful results. Keep secrets out of URLs and visual artifacts.

Inspect meaningful visual changes in rendered form when possible. Source inspection is not visual verification; screenshots are not functional-flow proof. If rendering is unavailable, complete supported work and state specific gaps.

Batch inspection, fix meaningful findings, and confirm affected areas. Do not loop indefinitely for subjective polish. The polish limit does not convert unresolved correctness/safety issues into passes.

## 6. Record only what should outlive the task

Deliver the requested artifact with consequential decisions, evidence, and remaining unknowns. Do not produce documents for every component.

When a user requests durable project guidance, update its existing authoritative document or create a scoped DESIGN.md as Project design describes. Keep project facts and local exceptions there. Proposed decisions remain proposed; no filename or status edit proves approval or implementation.

General skill changes require a transferable lesson with conditions and exceptions, not one project's preference. Real usage improves the skill; it is not a prerequisite for first use.
