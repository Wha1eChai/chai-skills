# Verification

Read before selecting acceptance criteria for a meaningful UI change or review, then return to the selected checks at completion. Use a relevant subset; do not turn every task into a product audit. Ordinary advice needs a coherent recommendation, not a browser session.

## Match evidence to the deliverable

| Deliverable | Appropriate checks | Completion does not mean |
| --- | --- | --- |
| Advice or decision proposal | Clear recommendation, reasoning, tradeoffs, assumptions, scope | Approved direction or implemented behavior |
| Component/page design specification | Structure, hierarchy, concrete states/actions, responsive intent, implementation-ready decisions or explicit open items | Rendered or functional validation |
| DESIGN.md / project baseline | Scope/status, specific actionable conventions, valid authority links, no duplicated value source, adoption criteria | Every page complies |
| Token/theme change | Source/mapping correctness, affected consumers, relevant themes/states and rendered checks when possible | JSON validity alone proves visual quality |
| Component/page implementation | Relevant task, visual, interaction, and code checks below | Production deployment or real-user acceptance |
| Review | Evidence and impact for findings; distinguish defects, choices, and gaps | Permission to apply fixes |

For an authorized design-only task, stop after delivering the design artifact and its criteria. For implementation, do not substitute a recommendation or unconsumed token file for working changes.

## Verification layers

### Task and meaning

- The principal task and necessary information are discoverable.
- Labels, units, time windows, scope, and action consequences match known facts.
- Loading, empty, failed, partial, and uncertain outcomes are not conflated.
- Important errors have a supported recovery or next step.
- Cross-page and asynchronous work preserves the required context.
- Examples, mocks, and unimplemented capabilities are not presented as real results.

### Visual craft

- Content is comfortable to read and scan; supporting information remains readily legible and discoverable. Assess rendered reading comfort as well as numerical accessibility thresholds.
- Important information and actions have a noticeable presence, with attention order and grouping that fit the task.
- Typography, color, imagery, spacing, density, and surfaces form an appealing, coherent expression suited to the audience and stated preferences. Identify what draws useful attention or invites continued reading, action, or exploration; assess with the user where subjective preference remains.
- Content works at realistic lengths; no hidden essential information or accidental clipping.
- Related components share visual and interaction vocabulary.
- Responsive structure preserves useful relationships rather than merely scaling down. When changing max-width containers, multi-column layouts, fixed regions, or breakpoints, select checks around the affected constraints taking effect—not only phone/tablet/desktop labels. Inspect shell, navigation, content, and local-outline relationships; distinguish intentional reading whitespace from accidental separation or obstruction. This is a targeted check, not a mandatory wider matrix for unrelated small edits.
- Decoration and motion support the direction instead of competing with the work.

### Interaction and accessibility

- Use semantic controls, accessible names, visible focus, and meaningful headings.
- Keyboard operation, focus return, and appropriate modal focus containment work.
- Account for IME composition when implementing keyboard shortcuts.
- Important actions are not hover-only or gesture-only.
- Fixed controls do not obscure content, errors, or focused elements.
- Verify text/background contrast in rendered states. WCAG AA generally requires 4.5:1 for normal text and 3:1 for large text, subject to criterion scope and exceptions. Large text is 18pt or 14pt bold (approximately 24 CSS px or 18.7 CSS px for typical Latin fonts), with equivalent-size provisions for CJK fonts; not 18px/14px.
- WCAG 2.2 AA target size minimum is 24×24 CSS px with specified exceptions, including spacing. A 44×44 CSS px target is a stronger touch-friendly starting point, not the universal AA minimum. Check actual hit regions and avoid overlap.
- Check zoom, reflow, long/localized content, and reduced-motion behavior as applicable. Contrast checks alone do not certify accessibility.
- Announce important asynchronous changes appropriately without overwhelming assistive technology with every polling update.

### Implementation

Use the smallest relevant checks: affected component tests, state/behavior regression, targeted build or typecheck when warranted, and rendered inspection for meaningful visual changes. Do not run unrelated broad suites or create a new test framework by default.

Preserve project dependency, permission, and operational boundaries. This skill does not authorize production actions, real payments, account creation, or external publication for validation.

## Evidence and reporting

Distinguish:
- Intended requirement.
- Observed source behavior.
- Rendered visual evidence.
- Functional interaction evidence.
- User-task evidence.

For substantial visual evidence, record enough context to interpret it: route/state, relevant viewport/theme, and version or build when available. Synthetic fixtures and local previews remain synthetic/local evidence.

When tools or environments are unavailable, report what was inspected and what remains unverified. Do not claim that code, screenshot, or automated accessibility output proves all other layers. Equivalent CSS viewport checks are not actual browser-zoom tests; label the method used.

A tool-side or local resource fetch failure does not establish unavailability in the target environment or authorize removing existing content/capabilities. Preserve the existing reference and report the limitation by default. Base replacement, hiding, or removal on an applicable confirmed requirement or further evidence within the authorized scope—not the local failure alone. This applies to images, fonts, video, embeds, and downloads. Test doubles prove only the behavior they exercise, not real remote availability, permissions, or integration.

Report findings as: observation and location → user impact → defect, design choice, or evidence gap → recommended action → focused verification. Avoid invented usability scores or efficiency percentages.

## Bounded self-review

Batch relevant views and states into one inspection pass, address meaningful findings together, then confirm the changed areas. Stop subjective polishing after that unless requested or a concrete unresolved issue justifies further work.

Do not change designs merely to ensure a second draft exists. Self-review may conclude that no revision is needed. Report remaining issues honestly; bounded polish never overrides correctness or safety requirements.
