# Project Design Baselines and System Evolution

Read when establishing or optimizing a project's design language, documenting DESIGN.md, consolidating recurring visual drift, or changing shared tokens/components. This is not required for every new page.

## Establish the requested artifact and authority

Distinguish these outcomes before editing:

| Outcome | Deliverable | Not implied |
| --- | --- | --- |
| Recommend a design direction | Short decision proposal with rationale, alternatives where material, and open assumptions | Files, tokens, implementation, or approved status |
| Document the existing design | Scoped observed baseline with sources and inconsistencies | Every existing choice is desirable or approved |
| Propose/improve a project standard | DESIGN.md or existing equivalent describing candidate direction, conventions, and adoption criteria | All pages now comply; authorization to redesign them |
| Adjust design tokens | Bounded machine-value/mapping change plus affected-consumer verification | New component library, full migration, or changed business behavior |
| Establish/evolve a reusable component | Reused/extended primitive or component, semantic variants, state contract, examples/tests | Replacing all similar controls or abstracting every one-off |
| Adopt a baseline in UI | Authorized representative component/page changes with evidence and remaining adoption scope | Site-wide rollout or production deployment |

For "optimize this project's design", inspect the existing system first. If the request does not establish whether the user wants a proposal, documents, or code, ask the narrow output-scope question. Do not ask for a comprehensive business interview. If the user explicitly requests documents/tokens or implementation, proceed within that scope without redundant approval.

## Workflow and timing

### 1. Inspect a bounded sample

Read applicable product/design guidance, theme configuration, token sources/adapters, component conventions, and a few representative surfaces. Identify their purposes and which files actually supply values.

Inspect enough to distinguish stable identity from accidental drift. Do not wait for a complete inventory, analytics, or user research. Mark source-only conclusions and runtime unknowns. Existing deployment/source variants may require a target decision, not an exhaustive historical audit.

**Working output:** authority map: intended guidance, observed implementation, value source, consumers, conflicts, and target surface. This can stay a short note unless durable inventory was requested.

### 2. Decide shared versus local

Read Surface and Style for expression/consistency and Taste for visual quality. Read Task and Layout only where navigation, density, comparison, or workflow conventions are in scope.

Choose:
- What stays: existing identity, accessible behaviors, useful patterns.
- What changes: specific drift or quality problems and their intended improvement.
- What is shared: semantic roles, component vocabulary, brand relationships.
- What varies: theme values, density, composition, reading width, surface-specific patterns.

Describe the intended reading comfort, attention priorities, and visual appeal, then connect these outcomes to concrete design relationships and useful examples. Identify recognizable brand anchors and which properties can evolve within scope; a color family can remain recognizable while its lightness or saturation changes. Separate observations, recommendations, and approved decisions. Only escalate unresolved choices with material cost or consequences.

**Output:** concise direction and scope. Do not force several alternatives when the requested direction is clear.

### 3. Write the smallest useful project contract

Prefer the existing authoritative document. Do not add a competing DESIGN.md solely for this skill. If no appropriate document exists and durable guidance is requested, use a scoped DESIGN.md at the relevant application/project boundary.

Useful contents:
- Scope and status: observed baseline, proposed target, approved target, or adopted areas.
- Surface purposes and existing product-context links; avoid duplicating business facts.
- Design intent, rationale, preserved identity, and allowed variation.
- Information/layout conventions and typography, density, color, depth, shape, motion roles.
- Existing component use, semantic variants, and important state conventions.
- Authoritative token/adapter paths; describe roles rather than copy all values.
- Applicable exceptions, unresolved decisions, and focused acceptance/adoption criteria.

This is a flexible checklist, not a mandatory schema. Omit irrelevant sections. An explicit user-selected direction can be recorded as selected, but implementation and verification remain separate facts. Document what adoption evidence exists and what does not.

In durable guidance, list a source as a decision basis only when it was actually inspected and supports the relevant decision. Put uninspected material under related reading or pending verification, not evidence. Distinguish observed facts, design inferences, and user decisions; reading a file does not validate all its claims. Use enough attribution to trace material decisions, not a citation for every sentence or a new source report for small edits.

**Stop here for documentation-only requests.** A useful baseline can ship now with candidate choices and gaps. Real usage will calibrate it; lack of a representative implementation does not invalidate the document.

### 4. Change tokens only when implementation authority includes them

Before changing shared values, read Verification and identify consumers, theme/mode overrides, component mappings, and potential blast radius.

- **Existing source:** edit the current authoritative values/config; do not add a second hand-maintained JSON mirror.
- **No source:** introduce only the values needed for authorized scope. CSS variables, a library theme, or project JSON may be enough; no mandatory DTCG/toolchain conversion.
- **Roles:** separate primitive values, semantic roles, and component-specific decisions only as needed. Avoid creating three layers for a tiny application.
- **Mapping:** ensure the actual library/theme/CSS adapter consumes the intended values. A token file with no consumer is a proposal artifact, not an applied system.
- **Naming:** prefer clear stable meaning; metaphorical names are optional, not proof of taste.
- **Migration:** preserve intentional exceptions, explain changed consumers, and use compatibility aliases where they reduce scoped migration risk. Avoid global search-and-replace across unknown semantics.

If only a token proposal is requested, show the proposed mapping/diff without activating it. If adjustment is requested, implement and verify the bounded mapping rather than returning values alone.

**Output:** actual source/mapping changes or an explicitly labeled proposal, affected scope, checks, and unverified states.

### 5. Compose or evolve components when requested

Check existing primitives and variants first. Define the component's semantic purpose, inputs/outputs, states, accessibility behavior, responsive behavior, and token use. Extract reusable structure only when real reuse or an established component-system requirement justifies it.

Deliver a component rather than merely a style table when working code was requested. Provide proportionate usage examples or existing story/test updates; do not install Storybook or another framework by default.

A sample/mock component may illustrate a direction, but does not prove API integration or production readiness. Do not implement new commercial or permission rules inside a design-system component.

### 6. Verify adoption, then update its record

For authorized implementation, select a representative affected component/page and relevant themes, content lengths, states, and widths. Prefer the smallest useful sample. Broad shared changes require a broader consumer check than local variants.

Check token resolution/mappings, functional states, and rendered hierarchy/contrast separately. Record only the areas actually adopted and verified. If runtime checks are blocked, preserve the exact supported result and residual gap; do not call the entire project standardized.

Finish with what changed, why, where the authoritative guidance/values live, evidence, and remaining adoption scope. Do not turn an initial baseline into a mandatory whole-site migration.

## Artifact boundaries

- **Decision note:** why a material choice was made; existing project decision location, or chat when persistence is not requested.
- **DESIGN.md:** human/agent-readable intent and conventions; not a runtime stylesheet or proof of adoption.
- **Tokens/theme:** machine-consumed values and roles; not a substitute for task or layout judgment.
- **Component:** reusable behavior and visual implementation; not a business-policy authority.
- **Evidence:** what was actually inspected/tested; separate from desired design.

One source per fact where practical. Link these artifacts instead of repeating the same values and business rules in all of them.
