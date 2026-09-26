# Provenance and Adaptation

This is an independently written synthesis for reusable, task- and business-aware interface design. It was originally developed in a project workspace; that workspace is historical context, not a runtime dependency or the subject of these rules. No upstream skill, CLI, hook, component library, or installation script is vendored here.

## Sources considered

| Source | Ideas adapted | Deliberately not inherited |
| --- | --- | --- |
| [Impeccable](https://github.com/pbakaus/impeccable), particularly its [skill](https://github.com/pbakaus/impeccable/blob/main/plugin/skills/impeccable/SKILL.md) and Operate guidance | Surface purpose, separating critique/audit/polish, task familiarity, bounded inspection | Runtime launcher, hooks, document prerequisites, absolute aesthetic bans, blanket boldness |
| [Interface Design](https://github.com/Dammyjay93/interface-design/blob/main/.claude/skills/interface-design/SKILL.md) | Task intent, hierarchy, density, spatial rhythm, component reuse | Mandatory domain/color inventories per task, unique-signature quotas, metaphorical token naming, rigid surface rules |
| [Anthropic frontend-design](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md) | Subject-aware visual direction, information-bearing structure, deliberate typography, restrained expressive emphasis | Novelty as a universal success criterion, automatic restyling of existing products |
| [Emil Design Engineering](https://github.com/emilkowalski/skills/blob/main/skills/emil-design-eng/SKILL.md) | Frequency/purpose-led motion, interaction continuity, optical details | Fixed output ceremony, mandatory press scaling, blanket easing and performance claims |
| [Taste Skill](https://github.com/Leonxlnx/taste-skill) | Brief interpretation, distinguishing preserve/redesign, independent expression dimensions | Numerical taste dials, default motion escalation, landing-page assumptions for operational UI |
| [Baseline UI](https://github.com/ibelick/ui-skills/blob/main/skills/baseline-ui/SKILL.md) | Concise implementation checks, existing primitives, local error feedback | Mandatory Tailwind/React libraries, unconditional color and animation restrictions |
| [Design & Taste](https://github.com/h3nryprod01/design-taste) | Reference routing as an organizational example | Direct aggregation of upstream rules, absolute anti-slop catalog, incorrect px/pt contrast threshold |
| User-supplied project design guidance (not redistributed) | Surface separation, honest states, scope/continuity, distinction between requirement and evidence | Project names, routes, commercial rules, token values, deployment authority, migration history |

These repositories evolve. The links identify research sources, not pinned dependencies or claims about all future versions. Maintenance should inspect current source rather than importing recommendations wholesale. If upstream text or code is copied in a future change, review that source's actual license and preserve required notices first.

## Standards and design-method references

- [WCAG 2.2 contrast minimum](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html): threshold scope, units, and equivalent text sizes.
- [WCAG 2.2 target size minimum](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html): AA minimum and exceptions.
- [GOV.UK patterns](https://design-system.service.gov.uk/patterns/) and [contribution criteria](https://design-system.service.gov.uk/community/contribution-criteria/): task-oriented patterns and evidence for reusable guidance.
- [NN/g design guidance](https://www.nngroup.com/articles/design-guidance/): distinction between principles, heuristics, and patterns.
- [Google DESIGN.md philosophy](https://github.com/google-labs-code/design.md/blob/main/PHILOSOPHY.md): design intent and rationale beyond token values.

Standards, contextual heuristics, and stylistic preferences have different authority. Do not present one as another.

## Positive-example sources and evidence

The optional [Positive examples](positive-examples.md) reference contains original synthetic scenarios, structural sketches, and reasoned alternatives informed by:
- [Carbon 2x Grid usage](https://carbondesignsystem.com/elements/2x-grid/usage/): style models, extra-width behavior, content alignment, and gutter relationships.
- [Carbon Typography overview](https://carbondesignsystem.com/elements/typography/overview/): productive/expressive type treatments within one design language.
- [GOV.UK Summary list](https://design-system.service.gov.uk/components/summary-list/) and [Check answers](https://design-system.service.gov.uk/patterns/check-answers/): single-object summaries, repeated-object cards, action scope, and edit-return continuity.
- [Carbon Motion overview](https://carbondesignsystem.com/elements/motion/overview/): productive/expressive moments and contextual motion choices.

Source prose and some example markup were inspected. Source screenshots and interactions were not independently visually/runtime verified; a direct Carbon image download attempt returned HTTP 403. No upstream assets/code are copied into the skill. The scenarios are adaptations, not vendor-endorsed examples or measured proof of effectiveness. They emphasize enterprise/public-service contexts and do not define all valid aesthetics. Source lookup is optional during ordinary use, not a network dependency.

## Authoring decisions

- General methods live in this skill; project facts are loaded only when relevant.
- Real projects improve the guidance through use, but are not a prerequisite for a first version or an ordinary task.
- Quality pursues readable content, salient priorities, visual appeal, and useful behavior together. Surface purposes guide attention rather than prescribing aesthetic intensity.
- Existing identity and familiar patterns provide anchors; the authorized design can evolve expressive properties around them. Explicitly approved values remain constraints until changed by agreement.
- Examples expand a design vocabulary; their palettes, structures, and paired alternatives are contextual teaching choices. The user's content and preferences can support other solutions.
- References are loaded by the requested artifact and unresolved decision triggers, not as one large mandatory context dump. Working notes do not automatically become files.
- Project design baselines, token proposals, applied mappings, reusable components, and adopted UI have different deliverables and evidence. Documentation is not rollout; implementation requests require implementation.
- Execution references are separate from skill maintenance and provenance.
- Small edits stay small. Reviews do not grant mutation authority.
- User-provided retrospective feedback and screenshot comparison informed focused refinements; the full execution transcript was not independently audited. Structural checks and synthetic scenario review remain distinct from runtime discovery, controlled generation benchmarks, and real-user validation.
